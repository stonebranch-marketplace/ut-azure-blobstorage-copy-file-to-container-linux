# ut-azure-blobstorage-copy-file-to-container-linux
# Universal Automation Center support for scheduling Azure Blob Storage cop file to container
# Abstract:

The here described Universal Tasks allow to Transfer and retrieve files from Azure Blob Storage in the Cloud. As a result, you can integrate any Azure Blob Storage file transfers into you existing or new scheduling workflows, providing a true hybrid cloud (on-premise and cloud computer) file transfer solution.

# 1.	Disclaimer

No support and no warranty are provided by Stonebranch GmbH for this document and the related Universal Task. The use of this document and the related Universal Task is on your own risk.

Before using this task in a production system, please perform extensive testing.

Stonebranch GmbH assumes no liability for damage caused by the performance of the Universal Tasks

# 2. Scope

This document provides a documentation how to install and use the Universal Tasks for Azure Blob Storage File Transfers. If more Task will be created in the future this document will be updated accordingly.  

# 3. Introduction

Storing data in the cloud becomes an integral part of most modern IT landscapes. With Universal Automation Center you can securely automate your AWS, Azure or any other Cloud File Transfer and integrate them into your existing scheduling flows.

As security is one of the blob concerns, when moving to the cloud, the provided solution supports multi-level of security:
  - All Credential for Azure Blob Storage are stored in an encrypted form in the database
  - Connections towards the Azure Blob Storage via a Proxy Server are supported

The here described Series of Universal Tasks focuses on the Azure Blob Storage file transfer. A similar solution as for Azure is also available for Amazon S3 storage. 

Some details about the universal tasks for Azure Blob Storage:
  - The Universal Tasks are calling the Microsoft Azure Storage SDK for Python 
  - The python azure-storage-blob module is called by a Universal Agent running on a Linux Server or Windows Server – Note: This document focuses on the Linux Version 
  - The Server Running the Universal Agent needs to have Python 2.7.x or 3.6.x installed
  - All Universal Task support encrypted connections via a Proxy Server
  - All Credential for Azure (account_name, account_blob) are stored in an encrypted form in the database
  - You can configure all connection Parameters for the Proxy and Azure via the Universal Task
  - You can select different log-levels e.g. Info and debug
  
The following Universal Task for Azure Blob Storage have been implemented: 
  

