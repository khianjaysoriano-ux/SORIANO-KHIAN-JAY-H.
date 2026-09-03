
# Core Components of Cloud Infrastructure

Cloud computing infrastructure relies on key abstraction layers that allow hardware resources to be delivered over the internet on-demand. Below are the three primary components:

---

## 1. Compute Resources
Compute resources represent the processing power of the cloud ecosystem. They host applications, process data, and execute operating systems.

* **Virtual Machines (VMs):** Software-based emulations of physical computers running guest operating systems managed by a hypervisor.
* **Containers:** Lightweight, isolated environments that package code and dependencies together, sharing the host machine's OS kernel.
* **Serverless Execution:** Event-driven compute platforms where code executes without manual server management or provisioning.

---

## 2. Storage Resources
Cloud storage provides reliable, scalable, and persistent data holding mechanisms tailored to different workload requirements.

* **Block Storage:** Direct-attached, high-performance storage volumes used primarily as virtual hard disks for virtual machines (e.g., operating systems and databases).
* **Object Storage:** Scalable storage designed for unstructured data (images, backups, media) accessible via unique HTTP/REST API endpoints.
* **File Storage:** Shared file systems accessible simultaneously across multiple virtual compute instances.

---

## 3. Virtual Private Cloud (VPC) & Networking
Virtual networking defines the isolated communication environment that connects cloud resources safely to each other and to the public internet.

* **Virtual Private Cloud (VPC):** An isolated, dedicated virtual network space within a public cloud tenant.
* **Subnets & Gateways:** Logical sub-sections of a network used to separate public-facing resources from private backend systems.
* **Security Groups / Firewalls:** Statefulness rules that act as virtual network firewalls to filter inbound and outbound traffic.
