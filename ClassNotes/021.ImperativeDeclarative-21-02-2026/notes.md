## 1. Project Overview and Architecture

The primary goal is to deploy a **3-tier application** that is "Sasta, Sundar, and Tikau" (Affordable, Elegant, and Durable).

* **Application Components**:
* 
**Frontend**: React-based UI (Monolith).


* 
**Backend**: Python-based API (Monolith).


* 
**Database**: The third tier supporting the backend.




* 
**Deployment Models**: Applications are generally categorized as **Monolithic (85%)** or **Microservices (15%)**.


* 
**Infrastructure Design**: Establishing a **Landing Zone (LZ)** is essential to handle Backup, Disaster Recovery (DR), Monitoring, Security, and Cost Optimization.


* 
**Types of LZ**: Simple Landing Zone or Hub and Spoke.





---

## 2. Infrastructure as Code (IaC): Imperative vs. Declarative

The diagram uses a pizza-making analogy to explain the two main ways to manage infrastructure (Resource Groups or "RG").

### Imperative Approach (The "Aunty" Method)

* 
**Concept**: You must provide step-by-step instructions (e.g., make the dough, roll it, add sauce).


* 
**Application**: Best for small projects.


* 
**Tools**: Uses CLI or PowerShell to execute specific commands in sequence.



### Declarative Approach (The "Gamche Wala" Method)

* 
**Concept**: You define the end goal (the "Menu") and the system figures out how to achieve it.


* 
**Example**: "I want 100 Resource Groups," and the tool creates them automatically.


* 
**Application**: Best for large-scale, complex work.



---

## 3. Cloud-Specific Automation Tools

Infrastructure can be managed manually or through automation across the three major cloud providers.

| Cloud Provider | Imperative Tools | Native Declarative Tools | Open Source (Declarative) |
| --- | --- | --- | --- |
| <br>**Azure** 

 | az cli, azure powershell 

 | ARM Templates, Bicep 

 | Terraform 

 |
| <br>**AWS** 

 | aws cli 

 | CloudFormation 

 | Terraform 

 |
| <br>**GCP** 

 | gcloud cli 

 | Deployment Manager 

 | Terraform 

 |

---

## 4. Why "Terraform is Rocket"

Terraform is highlighted as the superior choice for modern DevOps because:

* It is **Cloud Agnostic**: It knows how to build resources on every cloud.


* It supports **Multi-cloud** environments.


* It has strong **Open Source Community Support**.



> 
> **Note**: While manual "click-click" deployment is possible for Resource Groups, it is not recommended for scalable or professional environments.
> 
=