---
layout: page
title: Prerequisites
permalink: /prerequisites/
nav_order: 2
---

# Prerequisites
Check below steps before you use SSIS Catalog Migration Wizard for your first-ever migration.
{: .fs-6 .fw-300 }

1. SSISDB in the target SQL Server Integration Services Catalog already exists. If it does not exist, you can [create SSIS catalog](https://azureops.org/articles/create-ssis-catalog/) under the Integration 
Service Catalog on target SQL server.

2. You can inspect your SSIS Catalog to ensure consistency in the source SSISDB. The inspection result will provide details about possible errors or warnings. It would be best to fix them before you run the 
migration. Follow this [tutorial](https://azureops.org/articles/is-your-ssis-catalog-migration-ready/) to know more.

3. Make sure that the user running the wizard has the ssis_admin role on both source and target SSISDB.

{: .warning }  
Restoring an existing SSISDB on the target SQL Server may result in unexpected errors during or after the migrations.
