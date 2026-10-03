# Fictional Company Cloud Migration and Security Planning

## **Organisational background**
TechLink Solutions is a mid-sized technology company with approximately 350 employees operating across software development, data analytics, and digital services. The company currently hosts its applications and databases on an on-premises data centre located at its headquarters.

### **TechLink’s core system consists of:**
1. A customer-facing web application
2. A relational database storing customer and transaction data
3. Several internal services supporting analytics and reporting

Over the past two years, TechLink Solutions has experienced rapid business growth, resulting in increased system usage, unpredictable traffic spikes, and higher security expectations from clients.

### **Current IT Environment (Assumptions)**
* Infrastructure is fully on-premises
* Limited scalability due to fixed hardware capacity
* Manual server provisioning and patch management
* Basic perimeter security (firewalls, antivirus)  No built-in DDoS protection
* Limited disaster recovery (nightly backups stored on-site)
* Small IT team (8 staff), with moderate cloud knowledge
* No formal cloud governance framework

Recent outages caused by traffic surges and hardware failures have raised concerns among senior management regarding availability, security, and resilience.

## **Objectives**
1. Organisational Assessment
Assess TechLink Solutions’ readiness for cloud migration by identifying business drivers, evaluating the current IT infrastructure and its limitations, and assessing internal capabilities such as staff expertise and governance. Provide an overall readiness score with justification and identify areas requiring improvement before migration.

2. Cloud Adoption Strategy
Recommend an appropriate cloud deployment model and service model based on organisational needs. Identify suitable cloud providers and services, and propose a strategy for managing critical data and workloads with a focus on high availability, fault tolerance, and disaster recovery.

3. Security and Compliance Planning
Analyse key security risks associated with cloud migration, including data protection, identity and access management, regulatory compliance, and common threats such as insider attacks, malware, and DDoS. Propose a security framework that uses best practices and cloud-native security controls to mitigate these risks.

4. Migration Roadmap
Develop a phased migration plan outlining pilot testing, data migration, and full-scale deployment. Define timelines, milestones, and resource requirements, and address change management considerations such as staff training and communication.

5. Executive Summary and Presentation
Prepare an executive summary that consolidates the assessment findings, cloud strategy, security approach, and migration roadmap, clearly communicating the benefits, risks, and recommendations to senior management.

---

## **Case Study Scenario**
TechLink Solutions is migrating from an on-premises infrastructure to Microsoft Azure to improve scalability, availability, and security. You have been hired to design and deploy a secure cloud environment that supports internal services, protects against external threats, and uses containerisation for application deployment.

---

# Azure Cloud Infrastructure & Containerisation Tasks

## Task 1: Secure Cloud Network & Virtual Machines

### Objective
Create a secure Azure network environment that supports internal communication while limiting external access.

### Requirements
* **Virtual Network Setup:** Create an Azure Virtual Network (VNet) containing two subnets:
  * Application Subnet
  * Database Subnet
* **Virtual Machine Deployment:** Deploy two Virtual Machines within the Application Subnet.
* **Network Security Groups (NSGs):** Configure rules to:
  * Allow only necessary inbound traffic (HTTP/HTTPS, SSH).
  * Restrict database access strictly to internal network traffic.

### Evidence Required
* Screenshots of the VNet, subnets, and configured NSGs.
* Brief explanation of the applied security rules.

---

## Task 2: Database Deployment & Data Security

### Objective
Deploy a scalable database while ensuring complete security for both stored and transmitted data.

### Requirements
* **Database Deployment:** Create one of the following Azure database instances:
  * Azure SQL Database
  * Azure Cosmos DB
  * Azure Database for PostgreSQL
* **Security Controls:**
  * **Encryption at Rest:** Ensure data is encrypted while stored.
  * **Encryption in Transit:** Enforce Transport Layer Security (TLS).
* **Access Configuration:** Choose and configure one access strategy:
  * Allow Azure services (*simpler setup*) **OR**
  * Private Endpoint (*best practice*)

### Evidence Required
* Screenshots of the database configuration.
* Short explanation detailing the encryption mechanism and chosen access method.

---

## Task 3: Availability & Protection

### Objective
Ensure the application remains highly available and protected against malicious attacks.

### Requirements
* **Traffic Distribution:** Deploy an Azure Load Balancer or Application Gateway to distribute traffic.
* **DDoS Mitigation:** Enable Azure DDoS Protection (Basic/Infrastructure or IP/Network Protection).
* **Threat Explanation:** Briefly explain how these services mitigate:
  * High traffic loads
  * Distributed Denial of Service (DDoS) attacks

### Evidence Required
* Screenshots showing the Load Balancer/Application Gateway and DDoS settings.
* Short threat-mitigation explanation.

---

## Task 4: Containerisation with Docker

### Objective
Use Docker to package and deploy an application securely.

### Requirements
* **Docker Installation:** Install Docker on two Azure Virtual Machines.
* **Application Deployment:** Create and run a Docker container hosting a simple web application.
* **Secure Communication:** Demonstrate secure connectivity:
  * Between containers
  * With the database
* **Container Advantages:** Explain two key benefits of containerisation (e.g., scalability, resource efficiency, portability).

### Evidence Required
* Screenshots showing running Docker containers.
* Short written explanation covering container connectivity and key advantages.

---

## Task 5: Security Validation & Documentation

### Objective
Validate that security controls are functioning as intended and document the defensive posture.

### Requirements
Provide a brief written explanation detailing how each of the following components protects the cloud environment:
* **Network Security Groups (NSGs):** Filtering network traffic and maintaining subnet isolation.
* **Encryption:** Safeguarding data integrity and confidentiality at rest and in transit.
* **Load Balancer / Application Gateway:** Managing traffic distribution and preventing service saturation.
* **DDoS Protection:** Mitigating volumetric and application-layer denial-of-service attacks.
* **Containers:** Isolating application workloads and reducing attack surfaces.

### Evidence Required
* Documentation/written summary addressing each security control.
