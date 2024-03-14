---
layout: page
title: Getting started
permalink: /getting-started/
nav_order: 4
---

# Getting started
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

We will now see how SSIS Catalog Migration Wizard migrates on-premises SSIS Catalog in SQL Server to SSIS in Azure Data Factory in just a few clicks. I also have a video demo available to watch.

{% include youtubePlayer.html id="t2h6xNVFQkc" %}

To start, launch the wizard from your preferred location.

## Choose Source 
Choose the SQL Server radio button and then provide the SQL Server instance name. To perform operations on the SSIS catalog, we have to use Windows Authentication, and the user running this should have the ssis_admin role.

<img src="../media/ChooseSource.png" width="500">

## Choose Target
Choose the Azure data factory radio button for the target. Provide the Azure SQL Server hostname, admin SQL server authentication user name, and password.

<img src="../media/ChooseTarget.png" width="500">

{: .note }  
This utility only supports SQL authentication for the Azure SQL Server connection.

## Select SSISDB Catalog Items to Migrate
Choose the catalog items from the treeview.

<img src="../media/ChooseItems.gif" width="500">

### Compare source & target
Compare source and target and choose to migrate only what has changed.
For example, in the above image:
* Green items are present in the source and not present in the target,
* Red items mean source and target items are not the same.
* Unmodified items are displayed in the original color, and these objects are identical in the source and target

### Migrate only configuration
You can use this option to migrate only the project references and parameter values. Simply select the checkbox to migrate only the configuration part without the project code (.ispac file). Keep in mind that if the source project is not present in the target, both the project and its configuration will be migrated.
  
### Migration type
Migration types are ‘copy’ and ‘move’. Select the’ move’ radio button to delete the source catalog after the migration. The default type is ‘copy’.

### Migrate explicit permissions
Catalog folders, projects, and environments have explicit permissions. To migrate these permissions to the target, check the ‘Migrate explicit permissions' checkbox screen.

## Customize Folder Mapping
Easily map source and target its permissions' checkbox folder names. The wizard populates all selected folder names in the Source and Target folder columns. If you wish to customize the folders, edit the value in the ‘Target Folder’ column.

<img src="../media/CustomizeFolders.png" width="500">

For instance, as shown in the above image, the wizard will copy the content of the source catalog folder Pqr to the target catalog folder Abc. This step is optional.

## Replace Environment Variable and Parameter Values
Configure the key-value pairs you want to replace in the environment variable and parameter values. Suggest button will list suggestions for replacing values based on the selected Replace Scope. Click on the Ref column to view the affected environment variables and parameters as shown in the image below.

<img src="../media/ReplaceVariables.gif" width="800">

Perhaps, this is useful when setting up a parallel environment for your ETL workload, and some configuration is different in the target environment. This configuration is optional.

## Overwrite Environment Variable Values
The ‘Overwrite environment variable values’ setting recreates environment variables and parameter default values in the target. Note here that you may lose target data in this case.

## Export Sensitive Data
This setting applies to exporting SSIS Catalog to the SCMW file.SCMW export file is not encrypted—whenThe ‘Export sensitive data’ setting exports sensitive information in the export file as free text.

## Complete the Wizard
<img src="../media/Review.png" width="500">

Review the deployment summary. And if everything looks ok, click Finish.

## Monitor the Migration
<img src="../media/Finish.png" width="500">

Any warning or error during the migration gets shown next to the respective folder in the Result column tooltip of the grid. The success items are all noted as "Passed" in the above image.

