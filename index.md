---
title: About
layout: home
---

# SSIS Catalog Migration Wizard

SSIS Catalog Migration Wizard helps you migrate SSIS Catalog from one server to another It is an add-in for SSMS 18, 19, Visual Studio 2017, 2019 or 2022.
{: .fs-6 .fw-300 }

Migrate the SSIS catalog to the new server quickly using SSIS Catalog Migration Wizard. 

Do you want to:
* migrate SSIS to Azure Data Factory SSIS Integration runtime.
* migrate SSISDB from one server to another
* migrate SSIS catalog from SQL Server 2012 to SQL Server 2022 (or any version of SQL Server).
* migrate SSIS catalog environment variables from DEV to UAT etc.
*  restore SSISDB without master key.
* automate routine SSIS catalog migrations.

Then you are at the right place!

# Background

From SQL Server 2012 onwards, Microsoft introduced a new deployment model in SSIS called the project deployment model. This new model has many benefits in managing SSIS project deployments, executions, and configurations. With every new version of SQL Server, the SSIS Catalog is also getting upgraded with new features. In this article, I will describe how we can migrate the SSIS Catalog from one SQL Server instance to another using the SSIS Catalog Migration Wizard.

The SSIS Integration Services Catalog consists of the following artifacts:

* SSIS Builds (.ispac files) - Contains several SSIS packages with project and package parameters.
* Environments - Stores configurations of SSIS projects. These variables are used to configure the SSIS project and package parameters of SSIS projects.

