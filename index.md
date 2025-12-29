---
title: About
layout: home
nav_order: 1
---

# SSIS Catalog Migration Wizard

SSIS Catalog Migration Wizard helps you migrate the SSIS Catalog from one SQL server to another. It is an add-in for SSMS 18, 19, 20, 21, 22, Visual Studio 2017, 2019, 2022 and 2026. Additionally, it offers the flexibility to operate as an independent, standalone application.
{: .fs-6 .fw-300 }

[Get started now](https://ssiscataloger.azureops.org/download/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[View it on Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=AzureOps.ssiscatalogerpro){: .btn .fs-5 .mb-4 .mb-md-0 }

---

{% include youtubePlayer.html id="t2h6xNVFQkc" %}

## Supported Sources and Targets
- **SSISDB in SQL Server**: SSIS catalog enabled in SQL Server (2012, 2014, 2016, 2017, 2019, 2022, 2025). 
- **Azure Data Factory SSIS Integration Runtime (IR)**: This is used when running SSIS packages in Azure using Azure data factory pipelines.
- **SCMW export**: This is a unique export format for SSIS Catalog items.

## Key Features
- **Compare source and target catalogs**: Compare source and target and choose to migrate only what has changed.
- **Customize SSIS folder names on the go**: Quickly map source and target folder names. The wizard populates all selected folder names in the Source and Target folder columns. If you wish to customize the folders, edit the value in the ‘Target Folder’ column.
- **Replace SSIS environment variable values on the go**: Configure the key-value pairs you want to replace in the environment variable and parameter values with proactive suggestions.
- **Export, import, or delete SSISDB items in bulk**: Whether you want to keep the backup of SSIS catalog items or migrate SSISDB items to a different network or domain, SCMW file export covers this.
- **Inspect existing SSISDB for issues**: [Detect](https://azureops.org/articles/is-your-ssis-catalog-migration-ready/) critical issues in existing SSISDB before migration. 
- **Migrate catalog items to the same server**: Migrate SSIS Catalog items on the same SQL server but to different folders.
- **Automate activities with the command-line utility**: With the command-line utility, you can automate routine migrations in a few clicks. The migration script can be integrated with any scheduler or CI-CD tool.
- **Validate migrated projects automatically**: You can choose to validate all the migrated projects automatically after their migration.

## What objects can be migrated
- SSIS Catalog Folders.
- SSIS Build (.ispac) files.
- Environments and environment variables.
- Project and package parameter default values including connection manager properties and encrypted passwords.
- Project and package parameter server-side values including connection manager properties and encrypted passwords.
- Folder, project, and environment permissions.

## How It Works
- **Select the source**: Select the source SQL Server containing SSISDB to be migrated.
- **Provide the target**: Select the target SQL Server where you want to migrate SSISDB.
- **Manage migration settings**: Perform selection of SSISDB items and manage environment variables and parameter values update rules.

## Getting Started
1. **Install the Extension**: Get started by [installing](https://ssiscataloger.azureops.org/download.html)  the extension.
2. **Explore the Documentation**: [Refer](https://ssiscataloger.azureops.org/getting-started) to our detailed documentation for step-by-step guides.


