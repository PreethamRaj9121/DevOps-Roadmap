# ☁️ Top AWS Interview Questions for Freshers (Crack the 90% Bracket)

Welcome to the ultimate AWS Interview Preparation guide curated specifically for freshers and entry-level cloud/DevOps engineering roles. Most beginners focus purely on service names; this guide targets the operational mechanics and core architectures that interviewers actually test for.

---

## 🧠 Core Architecture & Networking

### Q1: What is the structural difference between an AWS Region and an Availability Zone (AZ)?
* **Answer:** 
  * A **Region** is a completely isolated geographic location somewhere in the world (e.g., `us-east-1` in N. Virginia) containing multiple data centers.
  * An **Availability Zone (AZ)** is a distinct, fully isolated data center (or cluster of them) *inside* that specific Region, equipped with redundant power, networking, and cooling. 
  * **The Goal:** You deploy resources across multiple AZs within a single Region to ensure high availability and absolute fault tolerance if one data center goes offline.

### Q2: Explain the difference between Security Groups and Network Access Control Lists (NACLs).
* **Answer:** They form the layers of defense in your Virtual Private Cloud (VPC), operating at entirely different levels:

| Feature | Security Group (SG) | Network ACL (NACL) |
| :--- | :--- | :--- |
| **Operating Layer** | Instance Level (acts as a firewall for an EC2 instance) | Subnet Level (acts as a firewall for the entire subnet) |
| **State Nature** | **Stateful:** Return traffic is automatically allowed, bypassing rule checks. | **Stateless:** Return traffic must be explicitly allowed via outbound rules. |
| **Rule Support** | Supports **Allow** rules only (everything else is denied by default). | Supports both **Allow** and **Deny** rules. |
| **Evaluation** | Evaluates all rules before deciding to allow traffic. | Evaluates rules in strict numerical order (lowest to highest). |

### Q3: How can an EC2 instance inside a private subnet download software updates from the internet securely?
* **Answer:** By leveraging a **NAT Gateway (Network Address Translation)**. 
1. You deploy a managed NAT Gateway inside the **public** subnet of the VPC.
2. You modify the route table of the **private** subnet to direct all outbound internet traffic (`0.0.0.0/0`) straight to that NAT Gateway.
3. The NAT Gateway forwards the request to the internet, receives the update, and passes it back to the private instance. The instance remains completely invisible to direct inbound connections from the open web.

---

## 🖥️ Compute & Storage Mechanics

### Q4: When should you choose Amazon S3 over Amazon EBS?
* **Answer:** 
  * **Amazon S3 (Simple Storage Service):** An object storage service built for unstructured data (images, backups, static web assets). It is globally accessible via an API/URL, scales infinitely, and does not need to be attached to a specific operating system.
  * **Amazon EBS (Elastic Block Store):** A persistent raw block storage volume intended for direct attachment to a single EC2 instance. It acts exactly like a local physical hard drive or SSD used to run operating systems, file systems, and heavy-duty transactional databases.

### Q5: What happens to the data on an EC2 instance when it is Stopped vs. Terminated?
* **Answer:** 
  * **Stopped:** The virtual machine shuts down, and you stop paying for compute hours. However, the data stored on the attached EBS root volume is preserved entirely. You continue to pay a minimal cost for the EBS storage space.
  * **Terminated:** The instance is permanently deleted. By default, the attached EBS root volume is deleted along with it unless the `DeleteOnTermination` attribute was explicitly turned off during initialization.

### Q6: What are EC2 Spot Instances, and what is their primary trade-off?
* **Answer:** Spot Instances allow you to bid on spare, unused AWS compute capacity at steep discounts (up to 90% off standard On-Demand pricing). 
  * **The Trade-off:** AWS can reclaim these instances with a brief 2-minute warning whenever they need the capacity back. They are ideal for fault-tolerant, flexible, or interruptible workloads like big data processing batch jobs, background queues, and test testing environments.

---

## 🔒 Security & Access Management

### Q7: Explain the difference between an IAM User and an IAM Role.
* **Answer:** 
  * **IAM User:** A permanent identity created within your AWS account representing a specific person or application (assigned a unique username, password, and long-term access keys).
  * **IAM Role:** A temporary identity that does not have permanent passwords or access keys. Instead, it is dynamically assumed by trusted entities (like an EC2 instance or an external AWS service) to obtain short-lived cryptographic security credentials to execute tasks safely.

### Q8: What is the AWS Shared Responsibility Model?
* **Answer:** It defines who is responsible for security configurations within the cloud ecosystem:
  * **AWS is responsible for Security "OF" the Cloud:** Safeguarding the physical infrastructure, global network systems, hardware, facilities, and core software layers running AWS services.
  * **The Customer is responsible for Security "IN" the Cloud:** Managing data encryption, configuring proper Network Access Control lists, applying OS patches on EC2 instances, and defining tight identity access privileges via IAM.

---

## 🛠️ How to Use This Repository
1. **Fork** this repository to your profile.
2. Read through the scenarios and try to explain them aloud—technical articulation is exactly what interviewers evaluate.
3. If you find this breakdown helpful, star ⭐ this repository to help other freshers break into cloud engineering!

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=PreethamRaj9121&label=Repo%20Views&color=0e75b6&style=flat" />
</p>
