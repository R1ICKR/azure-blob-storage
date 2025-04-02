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

---

### **Step 2: Create a Blob Storage Container**  
1. Open the newly created **Storage Account**.  
2. Navigate to **Containers** under **Data storage**.  
3. Click **+ Container**, enter a **name** (e.g., `mycontainer`), and choose an **Access Level**:  
   - **Private**: Only the owner can access.  
   - **Blob**: Public read access.  
   - **Container**: Public read access to all blobs inside.  
4. Click **Create**.  

---

### **Step 3: Upload a File to Blob Storage**  
1. Open the **Container** created earlier.  
2. Click **Upload** → **Select a file** (e.g., `.txt`, `.jpg`, `.csv`).  
3. Configure **Blob Type** (default is **Block Blob**).  
4. Click **Upload**.  

---

### **Step 4: Generate a Shared Access Signature (SAS) URL** *(Optional - Secure Access Sharing)*  
1. In the **Storage Account**, go to **Shared Access Signature (SAS)**.  
2. Select **Permissions** (Read, Write, Delete, etc.).  
3. Set an **Expiration Time** for temporary access.  
4. Click **Generate SAS and Connection String**.  
5. Copy the **Blob SAS URL** and share it for secure file access.  

---

## **Conclusion**  
This lab demonstrated how to create an **Azure Storage Account**, set up a **Blob Storage container**, and manage data through the **Azure Portal**. Azure Storage ensures **scalability, security, and high availability**, making it an ideal solution for cloud storage needs.
