# Case Study Scenario

TechLink Solutions is migrating from an on-premises infrastructure to Microsoft Azure to improve scalability, availability, and security. You have been hired to design and deploy a secure cloud environment that supports internal services, protects against external threats, and uses containerisation for application deployment.

---

## Azure Cloud Infrastructure & Containerisation Tasks

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
