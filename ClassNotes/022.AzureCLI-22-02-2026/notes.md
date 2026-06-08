## 1. Interaction with Azure

There are two primary ways to interact with Azure resources:

* 
**Manual (GUI Based):** Using the Azure Portal to perform tasks via "Click Click," which is described as a "boring" and non-automated process.


* 
**Tool (CLI Based):** Using a Command Line Interface—referred to as "kali kali screen" (black screens)—to execute commands.



---

## 2. Infrastructure Management Styles

The document categorizes automation into two distinct philosophies:

### Imperative (Step-by-Step)

* Requires providing specific, step-by-step instructions to the system.


* 
**Primary Tool:** Azure CLI.



### Declarative (Goal-Oriented)

* The user simply "declares" the desired end state, and the tool handles the execution automatically.


* 
**Primary Tool:** Terraform.



---

## 3. Azure CLI Fundamentals

The Azure CLI acts as a "wrapper" or "Meethi Goli" (sweet pill) for the **Azure REST API**, making it easier to send requests like `/vm/create` to the **Azure Resource Manager (ARM)**.

### Installation and Setup

* 
**Installation:** Download the `.msi` installer from Google/Microsoft and follow the "Next-Next" installation wizard.


* 
**Verification:** Open PowerShell and type the tool's short-hand keyword: `az`.


* 
*Comparison:* AWS uses `aws`, and Google Cloud uses `gcloud`.




* 
**Authentication:** Use the command `az login` to authenticate with your Azure account.



### Common Commands

To learn how to use any CLI tool, the document suggests using the help flag: `az --help`.

| Task | Command |
| --- | --- |
| **List Subscriptions** | <br>`az account list` 

 |
| **Set Active Subscription** | <br>`az account set` 

 |
| **Create Resource Group** | <br>`az group create` 

 |
| **View Resource Groups** | <br>`az group list` or `az group show` 

 |

---

## 4. Automation Goals

The document outlines a path toward full automation by:

1. Writing generic code for resources.
2. Implementing **CI/CD** (Continuous Integration/Continuous Deployment).
3. Setting a **Branching Strategy** to complete the automation lifecycle.



It concludes with an encouraging note: *"Manav jab jor lagata hai, patthar pani ban jata hai"* (When a human puts in effort, even stone turns to water).