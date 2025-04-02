# **Azure Storage (Blob Storage) Lab**  

## **Summary**  
Azure Storage Accounts enable secure and scalable cloud storage solutions. This lab provides step-by-step guidance on creating a storage account, configuring Blob Storage, and securely managing stored data. With flexible access controls and cost-effective redundancy options, Azure Storage is widely used for applications requiring high availability and durability.  

---

## **Lab Requirements**  
- **Azure Account** (Free Tier eligible)  
- **Internet Access** to navigate the **Azure Portal**  
- **Web Browser** (Microsoft Edge, Google Chrome, or Mozilla Firefox)  
- **Basic Understanding of Azure Storage Concepts** (recommended but not required)  

---

## **What is Blob Storage?**  
Azure Blob Storage is a **highly scalable, cloud-based object storage service** designed for unstructured data such as images, videos, documents, and backups. It provides **low-latency access, high durability, and cost-efficient storage** for applications requiring extensive data storage and retrieval. Blob Storage supports three types of blobs:  
- **Block Blobs**: Optimized for storing large amounts of unstructured data.  
- **Append Blobs**: Ideal for logs and append-only data scenarios.  
- **Page Blobs**: Used for virtual hard disks and frequent read/write operations.

---

## **Who**  
Cloud engineers, IT administrators, and developers managing storage solutions in Azure.  

## **What**  
This lab demonstrates how to create and configure an **Azure Storage Account** and a **Blob Storage container** to store and manage data in the cloud.  

## **When**  
Used when storing files, backups, application logs, or media in Azure securely and at scale.  

## **Where**  
Performed in the **Azure Portal**, **Azure CLI**, or **Azure PowerShell**.  

## **Why**  
Azure Storage provides **scalable, durable, and cost-effective** cloud storage for unstructured data like documents, images, and logs.  

---

## **Step-by-Step Instructions**  

### **Step 1: Create an Azure Storage Account**  
1. Navigate to **Azure Portal** → **Storage Accounts**.  
![image](https://github.com/user-attachments/assets/a55c31e1-24f1-4193-8692-919e648a0ec6)

2. Click **+ Create**.  
![image](https://github.com/user-attachments/assets/aa78e0d4-9fdb-47d8-9a21-cba0bbd34ccf)

3. Select the appropriate **Subscription** and create or choose an existing **Resource Group**.  
4. Enter a **unique Storage Account name** (e.g., `mystorageaccountxyz`).  
5. Choose **Region** closest to the users for better performance.  
6. Under **Performance** Select **Standard: Remommended for most scenarios (general-purpose v2 account)**
7. Choose **Geo-Redundant storage (GRS)** for Redundancy
8. Click **Review + Create** → **Create**.  
![image](https://github.com/user-attachments/assets/781bb9c4-4c97-494c-967f-4378e99812e8)
![image](https://github.com/user-attachments/assets/c1fe950d-9bb2-48b7-bfef-d3cd3b8d8e6e)
![image](https://github.com/user-attachments/assets/ed23600d-dc64-4519-acef-6ddd98374b72)

---

### **Step 2: Create a Blob Storage Container**  
1. Open the newly created **Storage Account**.  
2. Navigate to **Containers** under **Data storage**.  
![image](https://github.com/user-attachments/assets/c1e086be-50f0-49d6-9525-355002a200dc)

3. Click **+ Container**, enter a **name** (e.g., `mycontainer`), and choose an **Access Level**:  
![image](https://github.com/user-attachments/assets/da1f4ded-e391-4f64-b8ec-9393f2ff653a)
![image](https://github.com/user-attachments/assets/56ea5ecd-b22d-49c2-9a67-5c95cf936a6d)
![image](https://github.com/user-attachments/assets/c92e08e8-c583-4008-a986-71d6182dd3c9)

---

### **Step 3: Upload a File to Blob Storage**  
1. Open the **Container** created earlier.  
2. Click **Upload** → **Select a file** (e.g., `.txt`, `.jpg`, `.csv`).  
![image](https://github.com/user-attachments/assets/12fa2c28-8b09-45c7-bf63-d82d2c433a3a)
![image](https://github.com/user-attachments/assets/ba0c06b1-d9d4-4847-9602-dcc0379857d1)

3. Configure **Blob Type** under **Advanced** (default is **Block Blob**).  
![image](https://github.com/user-attachments/assets/6b2429ea-4348-4702-ae69-bed300f8b305)

4. Click **Upload**.  
![image](https://github.com/user-attachments/assets/33388aec-65d2-48b0-82c5-698f059dc40e)

---

### **Step 4: Generate a Shared Access Signature (SAS) URL** *(Optional - Secure Access Sharing)*  
1. In the **Storage Account**, go to **Shared Access Signature (SAS)**.  
![image](https://github.com/user-attachments/assets/e8e49ed1-75ef-4631-a58e-d0cc762a9314)

2. Select **Permissions** (Read, Write, Delete, etc.).  
3. Set an **Expiration Time** for temporary access.  
![image](https://github.com/user-attachments/assets/03032147-d5a7-457b-aa32-995ce9b0e794)

4. Click **Generate SAS and Connection String**.  
5. Copy the **Blob SAS URL** and share it for secure file access.  

---

## **Conclusion**  
This lab demonstrated how to create an **Azure Storage Account**, set up a **Blob Storage container**, and manage data through the **Azure Portal**. Azure Storage ensures **scalability, security, and high availability**, making it an ideal solution for cloud storage needs.
