# Azure Storage (Blob Storage) Lab

## Lab Overview

In this lab, explore **Azure Blob Storage**, a scalable object storage service for storing unstructured data such as text, images, videos, backups, and much more. Learn how to create and configure Blob Storage containers, upload files, and access them programmatically.

This lab is designed for beginners to get hands-on experience with managing Blob Storage in Azure.

## Prerequisites

Ensure the following prerequisites are met:

- An active [Azure free account](https://azure.microsoft.com/en-us/free/). (Free storage up to 5GB is available within the free tier)
- Basic understanding of **Azure** portal and **Storage accounts**.

## Lab Goals

- Create a **Storage Account** in Azure.
- Set up a **Blob Storage** container.
- Upload files into the container.
- Access and manage the files.
- Understand storage tiers and Blob types.

## Steps

### Step 1: Sign in to the Azure Portal
1. Go to the [Azure Portal](https://portal.azure.com/).
2. Sign in with the **Azure account**.

### Step 2: Create a Storage Account
1. In the Azure portal, click on **Create a resource**.
2. In the search box, type **Storage Account**, then select **Storage Account - BlobStorage**.
3. Click **Create** to start the Storage Account creation process.
4. Fill in the following details:
   - **Subscription**: Choose the active subscription.
   - **Resource group**: Select an existing resource group or create a new one.
   - **Storage account name**: Provide a globally unique name for the storage account.
   - **Region**: Select a region close by.
   - **Performance**: Choose **Standard**.
   - **Replication**: Select **Locally redundant storage (LRS)**.
   - **Access tier**: Select **Hot** (ideal for frequently accessed data).
5. Click **Review + Create**, and then click **Create**.

### Step 3: Set Up a Blob Storage Container
1. Once the **Storage Account** is created, navigate to the storage account.
2. In the **Storage Account** pane, click on **Containers** under **Blob Service**.
3. Click on **+ Container** to create a new container.
4. Enter a **name** for the container (e.g., `myblobcontainer`).
5. Choose the **public access level** (private or blob).
6. Click **Create**.

### Step 4: Upload Files to the Container
1. Go to the newly created container and click on **Upload**.
2. Click **Browse for files** and select a file to upload (e.g., a text file, image, or PDF).
3. Once the file is selected, click **Upload** to upload the file to the container.

### Step 5: Access and Manage the Files
1. Once the file is uploaded, it will appear listed in the container.
2. Click on the file to view its properties, including the URL and metadata.
3. To download the file, click the **Download** button or use **Azure CLI** or **SDK** to access the Blob programmatically.

### Step 6: Explore Blob Storage Tiers and Types
1. **Blob Types**: Blob Storage supports three types of blobs:
   - **Block Blobs**: Ideal for text and binary data.
   - **Append Blobs**: Suitable for logging data.
   - **Page Blobs**: For storing virtual hard disks (VHD).
   
2. **Storage Tiers**: Azure provides different storage tiers to optimize costs:
   - **Hot**: Optimized for frequent access.
   - **Cool**: For infrequently accessed data.
   - **Archive**: For long-term data archiving.

Explore the **Hot** tier by default and switch to **Cool** or **Archive** for testing to see the cost implications.

### Step 7: Clean Up Resources
1. After the lab, delete the **Storage Account** and **Container** to avoid ongoing charges.
2. In the **Storage Account** pane, click **Delete** and confirm.

## Conclusion

In this lab, the following tasks were successfully completed:
- Created an **Azure Storage Account**.
- Set up a **Blob Storage container**.
- Uploaded and accessed files in **Blob Storage**.
- Explored the **storage tiers** and different **Blob types**.

Azure Blob Storage can now be used for scalable, secure, and cost-efficient storage of unstructured data.

## Next Steps

- Learn more about **Azure File Storage**.
- Explore **Azure Storage Explorer** to manage Azure storage resources locally.
- Automate storage tasks using **Azure Logic Apps** or **Azure Functions**.

## Resources

- [Azure Storage Overview](https://docs.microsoft.com/en-us/azure/storage/common/storage-introduction)
- [Quickstart: Create a storage account](https://docs.microsoft.com/en-us/azure/storage/accounts/storage-account-quickstart)
- [Azure Blob Storage Documentation](https://docs.microsoft.com/en-us/azure/storage/blobs/)
