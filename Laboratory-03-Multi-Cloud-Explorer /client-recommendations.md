
# Cloud Platform Recommendation Challenge & Decision Matrix

## Client Recommendations

### Client A – Startup Company
* **Recommended Platform:** Google Cloud Platform (GCP) or AWS
* **Recommendation Justification:**
  For a mobile app startup with rapid growth potential and limited budget, GCP (or AWS) offers excellent startup credits, low-cost serverless backends, and flat network pricing. GCP’s Firebase platform and Google Kubernetes Engine (GKE) allow developers to focus on building features without managing heavy infrastructure. This setup ensures that as the mobile application's user base expands, the backend seamlessly scales on demand without high upfront maintenance costs.
* **Suggested Services:**
  1. Google Cloud Run / Firebase (App Hosting & Backend)
  2. Cloud Firestore / Cloud SQL (Database)
  3. Google Cloud Storage (Media & Assets)

---

### Client B – University
* **Recommended Platform:** Microsoft Azure
* **Recommendation Justification:**
  Azure is the ideal choice for this university because it already relies heavily on Windows Server, Active Directory, and Microsoft 365. Migrating to Azure will allow seamless identity federation via Microsoft Entra ID (Azure Active Directory) without re-architecting user accounts. Furthermore, the university can leverage existing Microsoft licensing discounts (Azure Hybrid Benefit) to significantly reduce migration costs while keeping operations familiar for system administrators.
* **Suggested Services:**
  1. Microsoft Entra ID (Identity Federation & SSO)
  2. Azure Virtual Machines (Hosting Windows Server workloads)
  3. Azure SQL Database (Database Hosting)

---

### Client C – AI Research Company
* **Recommended Platform:** Google Cloud Platform (GCP)
* **Recommendation Justification:**
  GCP leads the market in high-performance computing specifically tailored for Artificial Intelligence and Machine Learning research. Their custom Tensor Processing Units (TPUs) provide faster training times for complex deep learning models compared to traditional computing architectures. Combined with Vertex AI and BigQuery, GCP delivers an end-to-end framework built specifically for processing data-intensive neural network models efficiently.
* **Suggested Services:**
  1. Vertex AI (Machine Learning Platform)
  2. Compute Engine with Cloud TPUs/GPUs (High-Performance Compute)
  3. BigQuery (Data Warehouse & Analytics)

---

### Client D – Global E-Commerce Company
* **Recommended Platform:** Amazon Web Services (AWS)
* **Recommendation Justification:**
  AWS provides an unmatched global footprint, high availability, and proven auto-scaling capabilities necessary for high-volume global shopping platforms. Amazon's history as an e-commerce giant means AWS services are explicitly optimized for peak shopping traffic, fraud prevention, and global content delivery. Utilizing multi-region database replication alongside CloudFront guarantees ultra-low latency and uninterrupted service for worldwide customers.
* **Suggested Services:**
  1. Amazon EC2 with Auto Scaling Groups & Application Load Balancers
  2. Amazon CloudFront (Global CDN for fast content delivery)
  3. Amazon Aurora (Global Relational Database with high availability)

---

## Multi-Cloud Decision Matrix

| Business Requirement | Recommended Platform | Justification |
| :--- | :--- | :--- |
| **Startup Company** | GCP / AWS | Low initial costs, developer-friendly serverless platforms, and high scalability. |
| **Enterprise Organization** | Azure / AWS | Proven enterprise support, robust compliance certifications, and hybrid options. |
| **Microsoft Environment** | Microsoft Azure | Direct integration with Active Directory, Windows Server, and license mobility. |
| **AI / Machine Learning** | Google Cloud Platform | Dedicated TPU hardware and industry-leading Vertex AI toolset. |
| **Kubernetes Deployment** | Google Cloud Platform | Managed GKE offers native, mature Kubernetes support straight from its creator. |
| **Global Web Application** | Amazon Web Services | Massive global footprint, extensive CDN network, and high availability features. |
