
# Cloud Storage Types Research

## Comparison of Storage Architecture

| Storage Type | Description | Primary Use Case | Cloud Provider Examples |
| :--- | :--- | :--- | :--- |
| **Block Storage** | Splitting data into fixed-sized blocks, each with a unique identifier. Operates like a raw, unformatted physical hard drive. | System boot volumes, high-performance databases (e.g., PostgreSQL, MySQL), transactional workloads. | AWS EBS (Elastic Block Store), Azure Managed Disks, GCP Persistent Disk |
| **File Storage** | Storing data in a hierarchical file-and-folder tree structure accessible over a local network. | Shared network drives, centralized user directories, legacy application migration. | AWS EFS (Elastic File System), Azure Files, GCP Filestore |
| **Object Storage** | Storing data as self-contained objects containing raw data, customizable metadata, and a unique global ID within a flat namespace. | Static web assets, media hosting (photos/videos), backup archives, unstructured big data. | AWS S3, MinIO, Azure Blob Storage, GCP Cloud Storage |

---

## Recommendation for Client Application

Object Storage is the ideal solution for storing user-uploaded images because it provides practically unlimited flat-namespace scalability without the file-system overhead of traditional block or file storage. Unlike container storage or block volumes, Object Storage decouples storage capacity from web server compute instances, allowing images to remain persistently accessible over HTTP/S APIs regardless of container lifecycles. Additionally, Object Storage enables custom metadata tagging and cost-effective scaling to millions of media assets.
