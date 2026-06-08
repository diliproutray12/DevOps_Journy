## 1. Azure Hierarchy and Structure

The document outlines the organizational flow of resources within Azure, comparing it to a banking system for easier understanding.

* 
**Entra ID & Management Groups:** The top-level identity and management layers.


* 
**Subscriptions:** Linked to billing and resource limits (e.g., a subscription with a balance of INR 18,000).


* **Resource Groups (RG):** Logical containers for resources. The document suggests creating these through both "Click Click" (Portal) and "AZ CLI" methods.


* 
**Global Uniqueness:** Specifically, an **Azure Storage Account name must be globally unique**.



---

## 2. Azure Storage Account ("The Digital Godown")

An Azure Storage Account is described as a "Digital Godown" (warehouse) used to store various types of data.

### Core Storage Services

There are four primary services provided by a Storage Account, categorized by the type of data and access method:

| Service | Data Type / Use Case | Access Method |
| --- | --- | --- |
| **Blob (Containers)** | Unstructured data like mp4, pdf, mp3, ppt, docx.

 | HTTP/HTTPS 

 |
| **File Share** | Shared file storage (e.g., 1TB capacity).

 | SMB 

 |
| **Azure Table** | Structured NoSQL data (e.g., ID, Name, Age).

 | HTTP/HTTPS 

 |
| **Azure Queue** | Messaging for asynchronous tasks using **First In, First Out (FIFO)**.

 | HTTP/HTTPS 

 |

---

## 3. Data Lifecycle Management (Blob Tiers)

Data within Blobs can be moved between tiers based on how often it is accessed to optimize costs.

* 
**Hot Tier:** For data that is accessed very frequently.


* 
**Cool Tier:** For data accessed less frequently.


* **Archive Tier:** For data that "just lies there," like a wedding video. It is rarely accessed but must be preserved.


* 
*Humorous Note:* "Everyone has it, but no one watches it".





---

## 4. Azure Regions, Zones, and Redundancy

The document uses a map of the United States (West US, Central US, East US) to explain how Azure handles physical infrastructure and data safety.

### Redundancy (Replication) Types

To prevent data loss, Azure offers different levels of replication:

* 
**LRS (Locally Redundant Storage):** All copies of the data are kept within a **single data center**.


* 
**ZRS (Zone Redundant Storage):** Copies are spread across **different zones** within a single region.


* 
**GRS (Geo-Redundant Storage):** Copies are made across **different regions** for maximum safety.



---

## 5. Key Interview Questions

The document concludes with essential topics for interview preparation:

* What is an Azure Storage Account? 
* Explain the Lifecycle Management of storage account data.
* What services are provided by a Storage Account? 
* What are the different Replication (Redundancy) types? 

