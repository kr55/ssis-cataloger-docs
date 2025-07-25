---
layout: page
title: Frequently asked questions
permalink: /faq/
nav_order: 8
---
# Frequently asked questions

## Licensing 

**How many users are available in one license?**

All SSIS Catalog Migration Wizard license editions offer multi-user access per server and grant access to all the users on the server or computer where it is installed.

**How many licenses do I need to buy for my SSISDB migration?**

You can migrate SSISDB between any SQL Servers from the server where the tool is installed. So, if your source and target SSISDB can be connected from a single server, you need only a single license.

**We are an educational institute or non-profit organization. Can we get any offer or discount on the license?**

We offer exclusive discounts to educational institutes and non-profit organizations. To check the offer, write an email to [support@azureops.org](mailto:support@azureops.org) from your official email address. The offer will be tagged to the official email address and can only be availed when using the email as the billing address.

**I am planning to purchase multiple licenses at the same time. Can I get a discount?**

We offer discounts to our customers planning to acquire more than two licenses simultaneously. To check the latest offer, email [support@azureops.org](mailto:support@azureops.org)
with your requirements. The offer code will be delivered to you based on your purchase plan.

## Technical 

**What all source and target SQL Servers are supported for migration of SSISDB.**

SSIS Catalog Migration Wizard supports migration of SSISDB between SQL Server 2012, 2014, 2016, 2017, 2019, 2022, ADF SSIS IR, and Azure SQL MI. It is recommended to only migrate the SSIS catalog from lower to higher versions of the SQL Server as features in SSIS may not be backward SQL server version compatible. 

**Does this tool migrate SSIS environment references?**

SSIS Catalog Migration Wizard migrates environment variables and project/package parameter server-side values from source to target SSISDB. Using a proactive recommendation process, you can also update their values during the migration.

**My source and target SSISDB are in different networks/domains and do not have a direct connection. Will SSIS Catalog Migration Wizard work in this case?**

SSIS Catalog Migration Wizard offers a .scmw file (an export format for SSISDB items). You can achieve SSISDB migrations across different domains. Export the source SSISDB in a .scmw file using SSIS Catalog Migration Wizard. Copy this file to the target server or computer where you have access to the target SQL Server (SSISDB). Import the scmw file to target SSISDB using SSIS Catalog Migration Wizard. Please note that you need to install SSIS Catalog Migration Wizard in source and target network machines. Learn more about it [here](https://azureops.org/articles/export-and-import-ssisdb/).

**How can I ensure that my source and target servers can be connected from the wizard?**

SSIS Catalog Migration Wizard uses native SQL connection API to connect to SQL Servers. If you can connect to source and target SQL servers using other client tools like SQL Server Management Studio, the connections should also work from the wizard. You can also try the connections by downloading the SSIS Catalog Migration Wizard from [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=AzureOps.ssiscatalogerpro&ssr=false#overview).

**I do not have the SSISDB master key. Can I still migrate my SSISDB to target SQL Server SSISDB?**

You do not need to provide the master key of source SSISDB to migrate your SSISDB to the target SQL Server using SSIS Catalog Migration Wizard.

**Can I migrate SSIS Catalog objects on the same server but in different folders?**

You can select the same source and target server on the screens and choose different folders. 

**Can I migrate the SSIS project configuration to the new SSISDB without migrating the project?**

It is possible to migrate SSIS project parameter values and environment configuration without migrating the project itself by using the 'Migrate only configuration' setting. However, the wizard will also migrate the project definition if the target does not already have the project.

**Can the tool migrate sensitive environment variables and parameter values in my SSISDB?**

Yes, SSIS Catalog Migration Wizard fully supports the migration of sensitive data, including environment variables and project/package parameter values, to the target SSISDB. Your sensitive values will be securely transferred during the migration process.

**Is this tool capable of migrating .NET script tasks?**

SSIS Catalog Migration Wizard does not change the build (.ispac) file during the migration from a lower to a higher version of SSISDB. Usually, script tasks are backward compatible. However, it is advisable to consult support at [support@azureops.org](mailto:support@azureops.org) for a limited feature free trial to validate if it works for you.

## Software package and policies

**What has been included in the software package?**

You will receive an email with a download link to the product and an activation key. Once you download the zip file after the purchase, you will get an installer to install and activate the software, installation guide, and product documentation file. 

**I am facing issues with the migration; how can I get help?**

The AzureOps support team offers dedicated support to SSIS Catalog Migration Wizard users. You can contact a support agent from the product page live chat or email [support@azureops.org](mailto:support@azureops.org) with the problem statement.

**Does SSIS Catalog Migration Wizard require an internet connection to work?**

SSIS Catalog Migration Wizard is an offline tool; hence, it does not require the Internet to work. The Installer of the tool interacts with the Licensing server only once over the Internet.

**What payment options are available?**

We currently only accept payment via PayPal. If you do not have a PayPal account, PayPal generally offers to use a credit card without creating an account. However, this differs based on your country of origin. Check out PayPal [privacy policy](https://www.paypal.com/us/legalhub/privacy-full). Reach out to our support in case of any payment issues.
 
**Does this tool come with a refund policy?**

SSIS Catalog Migration Wizard migrates SSIS Catalog from one server to another in just a few clicks. If it does not work for you and you wish to get a refund, you can claim it within three days of the purchase. Check out our [refund policy](https://azureops.org/refund_returns/) for more details.

**Is there a limited feature free trial available?**

Yes, you can download the free trial of SSIS Catalog Migration Wizard from the [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=AzureOps.ssiscatalogerpro). The trial version allows migration of the first 3 SSIS items from the source to the target SSISDB.

**How can I receive software updates?**

AzureOps offers free software updates readily available on the Visual Studio marketplace. If you installed this tool as a Visual Studio extension, these updates will be automatically shipped to you. However, if you do not have extensions, you can download the updates anytime from the marketplace. 

