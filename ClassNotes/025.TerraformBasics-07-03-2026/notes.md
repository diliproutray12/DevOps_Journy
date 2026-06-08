## 1. Community Guidelines & Onboarding

The Siksha Sathi program follows a strict community-driven approach with specific behavioral and administrative rules.

* **Communication Rules:** A professional decorum is required; "Good morning/night" messages, personal "baby shona" talk, or "did you eat" messages are strictly prohibited.


* 
**Account Responsibility:** Members must create their Azure accounts during their assigned month. Failure to do so results in a ₹1000 penalty to be paid to group members via UPI.


* 
**Support System:** Every student is assigned two mentors from previous batches who work at major MNCs like Microsoft and Mastercard.


* **Key Contacts:**
* 
**Registration:** Ravi Sir.


* 
**SRD & Group Assignment:** Anubhav Sir.


* 
**Access Issues:** If Cloudflare or Azure credentials are not received by the deadline (Wednesday/EOD), contact Anubhav Sir.





---

## ## 2. Learning Progression (The "Story So Far")

The curriculum progresses from manual setups to advanced automation tiers:

1. 
**Tier 1:** Windows IIS.


2. 
**Tier 2:** Killercoda.


3. 
**Tier 3:** DevOps Insiders Cloud.


4. 
**Tier 4:** Azure Cloud.



> 
> **Important Instruction:** Users are forbidden from using Chatbots until they have manually created 20–25 resources and mastered the core concepts. Concepts should be learned via chatbots, but code must be written using Google or official documentation.
> 
> 

---

## ## 3. Azure Infrastructure Tasks

Upon receiving access, members must perform the following sequence:

* 
**Verification:** Check access in the portal; you must have **Contributor** permissions.


* 
**Resource Group (RG):** * First, create an RG manually via the Azure Portal.


* Second, create an RG using the **Azure CLI** (`az group create`).




* 
**Storage Account:** Create this manually after reading the documentation.


* 
**Core Concept:** Focus on understanding the **Region vs. Zone** architecture.



---

## ## 4. Infrastructure as Code (IaC) & Automation

The documentation distinguishes between two primary methods of managing resources:

### ### A. Imperative (Azure CLI)

* 
**Approach:** You tell the system *how* to do it step-by-step.


* 
**Process:** Install CLI → `az login` → Run commands → RG is created.



### ### B. Declarative (Terraform & Others)

* 
**Approach:** You define the *desired state* (the "what"), like an architect designing a 5 BHK house.


* **Tools Comparison:**
* 
**ARM Templates:** Described as a "Fisaddi" (ineffective/clumsy) tool.


* 
**Bicep:** A decent tool but limited strictly to Azure.


* 
**Pulumi:** Supports standard languages like Java and Python.


* 
**Terraform:** The preferred industry-standard tool.





---

## ## 5. Deep Dive: Terraform

Terraform is an open-source IaC tool created by HashiCorp (now owned by IBM).

### ### Why Use Terraform?

* Written in **Go** language.


* Offers **Multi-Cloud Support** (not locked into Azure).


* Features robust **State Management**.


* Strong open community support.



### ### How Terraform Works

1. 
**Language:** Uses **HCL** (Hashicorp Configuration Language), which is designed to be very easy.


2. 
**Configuration:** You create a file (e.g., `chameli.tf`) and define the resource.


3. **Execution:**
* Install Terraform.

* Run `az login` to authenticate.

* Run Terraform commands to deploy the Resource Group.

