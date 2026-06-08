# 📘 DevOps Insiders – Batch 18 Notes

---

# 🔥 1. How to Solve Any Doubt (Very Important Flow)

When you get stuck, follow this **step-by-step escalation approach**:

### 🧠 Step 1: Self Effort (Mandatory)

* Google at least **20 pages**
* Try tools:

  * ChatGPT
  * Gemini
  * Claude.ai

👉 *Goal: Build problem-solving mindset*

---

### 👥 Step 2: Community Support

* Ask in **Siksha Sathi Group**
* Ask in **B18 Main Group**

---

### 👨‍🏫 Step 3: Mentors

* Contact:

  * Anubhav Sir
  * Atul Sir (Technical)
  * Ashish Sir

---

### 🧑‍💻 Step 4: Advanced Help

* Seniors / Previous batch experts will help

---

### 🎯 Final Level

* If still interested → Watch all course videos (500+ videos)

---

# 🚀 2. For New Joiners

### 📌 Mandatory Steps:

1. Watch **last Sunday’s 3.5-hour video**
2. Attend upcoming Sunday session
3. Catch up with batch progress
4. Use groups if stuck

---

# 🧠 3. Learning Strategy (MOST IMPORTANT)

❌ Don’t:

* Re-watch videos repeatedly
* Focus only on theory

✅ Do:

* Recall from memory
* Practice assignments
* Think logically

👉 Reason:

* Course has **500+ videos (2.5+ hrs each)** → Impossible to rewatch all

---

# 🏗️ 4. Architecture Evolution

### 🟢 Stage 1: 1-Tier Architecture

* Everything on one system

---

### 🟡 Stage 2: 3-Tier Monolithic

* Frontend
* Backend
* Database

---

### 🔵 Stage 3: 3-Tier Microservices

* Services split into independent units
* Scalable + flexible

---

### ⚙️ Technologies Involved:

* Virtual Machines
* App Services
* Load Balancer
* Application Gateway
* Azure Front Door

---

### 📦 Containerization:

* AKS (Azure Kubernetes Service)
* ACS

---

### 🤖 4th Tier (AI Layer)

* ML Model Integration
* Data Scientist:

  * Writes model
  * Data training
  * Deployment

---

### 🧠 Future:

* Agentic AI Applications
* LLMOps (Large Language Model Operations)

---

# ☁️ 5. Azure Basics

### 🔑 Login Steps:

* Go to: `portal.azure.com`
* Setup **MFA**

---

### 🔐 Access Check:

* Go to **Entra ID**
* Verify:

  * User exists
  * Role = **Contributor on Subscription**

---

### 🏢 Azure Hierarchy

```
Tenant Root Group
   ↓
Management Group
   ↓
Subscription
   ↓
Resource Group
   ↓
Resources (Storage, VM, etc.)
```

---

### 📦 Resource Group

* Logical container (like a “thela” 🛒)
* Holds all resources

---

### 📁 Storage Account Services:

* Blob
* File Share
* Table
* Queue

---

# ⚙️ 6. Ways to Create Resources

### 🖱️ Manual

* Azure Portal (click-click)

---

### 💻 Automation

* Azure CLI
* Terraform

---

### 🧭 Approaches

| Type        | Meaning               |
| ----------- | --------------------- |
| Imperative  | Step-by-step commands |
| Declarative | Define desired state  |

---

# 🧱 7. HLD (High Level Design)

Before implementation:

* Design architecture
* Define:

  * Resources
  * Structure
  * Dependencies

---

# 🏗️ 8. Terraform Fundamentals

### 📌 What is Terraform?

* Tool by **HashiCorp**
* Used to write **Infrastructure as Code (IaC)**
* Works across:

  * Azure
  * AWS
  * GCP
  * Oracle

---

### 📂 Terraform Configuration

* File extension: `.tf`

---

### 📦 Core Concepts

#### 🔹 Resource

Example:

* Resource Group
* Storage Account

---

#### 🔹 Arguments

| Type     | Example        |
| -------- | -------------- |
| Required | name, location |
| Optional | tags           |

---

# 🔌 9. Providers (VERY IMPORTANT)

### 📌 What is Provider?

* Plugin that connects Terraform to cloud

👉 Example:

* Azure → AzureRM Provider
* AWS → AWS Provider

---

### 💡 Simple Analogy:

👉 Provider = **Middleman (Dalla)** between Terraform & Cloud

---

### ⚙️ Provider Setup Steps:

1. Install Terraform
2. Install Provider
3. Set Environment Variables

---

# 🖥️ 10. Installation Paths

Example:

```
C:/tools/terraform.exe
```

---

# 📚 11. Terraform Registry

Official docs:
👉 [https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs)

📌 Must read at least once

---

# ⚡ 12. Terraform Workflow

### 🔁 Steps:

1. Write `.tf` file
2. Run:

   ```
   terraform init
   terraform validate
   terraform plan
   terraform apply
   ```

---

### 📌 Important Notes:

* Terraform scans `.tf` files in folder
* If no `.tf` file → error
* Commands work based on file content

---

# 🔗 13. Dependencies

* Every system needs dependencies before running
* In Terraform → handled via **Providers**

---

# 💻 14. Azure CLI + Terraform Flow

### Steps:

1. Install Terraform
2. Install Azure CLI
3. Login:

   ```
   az login
   ```
4. Create:

   * Resource Group
   * Storage Account

---

# 🧪 15. Development Setup

### 📝 Option 1: Notepad

### 🧑‍💻 Option 2: VS Code (Recommended)

* Install Terraform Extension
* Create:

  * Folder
  * `.tf` file

---

### 📁 Example Workflow:

1. Create folder
2. Open terminal
3. Navigate:

   ```
   cd folder-name
   ```
4. Write Terraform code
5. Run commands

---

# 🧠 16. Key Understanding

* Terraform = **Declarative**
* Azure CLI = **Imperative**
* Portal = **Manual**

---

# 🎯 17. Important Philosophy

* Everyone will become a **teacher**
* Learn → Practice → Teach

---

# 🧩 18. Key Terms Recap

* HLD → High Level Design
* IaC → Infrastructure as Code
* Provider → Cloud connector
* Resource → Infrastructure component
* Arguments → Inputs to resource

---

# 🚀 Final Takeaway

👉 Focus on:

* Practice over theory
* Community learning
* Real-world architecture

👉 Goal:
**1-Tier → Microservices → AI-enabled systems**
