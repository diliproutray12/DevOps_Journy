# Terraform Basics – Batch 18 Notes



## 1. Objective of the Session

The goal of this session is to understand how **Infrastructure can be created using Terraform instead of manually creating resources in the cloud**.

Terraform reads a **configuration file** and automatically provisions the required infrastructure.

Example:

* Instead of manually creating a **Resource Group in Azure**, we will write a **Terraform file** and Terraform will create it for us.

---

# 2. What Terraform Does

Terraform works using **Infrastructure as Code (IaC)**.

Steps:

1. We write infrastructure configuration in a **file**.
2. Terraform **reads the file**.
3. Terraform communicates with the **cloud provider (Azure)**.
4. Terraform creates the **infrastructure automatically**.

Example:

```
Create Resource Group
Create VM
Create Storage
Create Network
```

Everything can be written in **one configuration file**.

---

# 3. Folder Structure to Create

Inside your computer create the following structure.

### Step 1: Create Main Folder

Create a folder named:

```
DevOps-Insiders
```

### Step 2: Create Subfolders

Inside it create:

```
DevOps-Insiders
│
├── Terraform
│
└── rg-using-terraform-07-03-2026
```

This is where your Terraform project will live.

---

# 4. Creating Terraform File

### Step 1

Go inside the folder:

```
rg-using-terraform-07-03-2026
```

### Step 2

Right Click

```
New → Text Document
```

### Step 3

Rename the file.

Example:

```
main.tf
```

Important rule:

Terraform only understands files with extension:

```
.tf
```

Example valid names:

```
main.tf
rg.tf
azure.tf
terraform.tf
```

---

# 5. Opening the Terraform File

Steps:

1. Right Click on the file
2. Select

```
Open With → Notepad
```

Now you can write Terraform code inside it.

---

# 6. What Should Be Written Inside the File?

Inside the `.tf` file we will define infrastructure.

Example idea:

```
Create Resource Group
```

Terraform will read this file and automatically create the resource group.

Important concept:

We **declare infrastructure** in the file.

Example concept:

```
Infrastructure declaration
```

---

# 7. Installing Azure CLI

Terraform needs authentication with Azure.

So we install **Azure CLI**.

### Steps

Go to Google and search:

```
Install Azure CLI
```

Download:

```
MSI Installer
```

Installation process:

```
Next
Next
Next
Finish
```

---

# 8. Azure CLI Commands

After installing Azure CLI, open **PowerShell** and run:

### Check Azure CLI

```
az --help
```

### Login to Azure

```
az login
```

This will open the browser and allow you to sign into your Azure account.

---

# 9. Installing Terraform

Steps:

Search in Google:

```
Install Terraform
```

Download Terraform for Windows.

Example downloaded file:

```
terraform_1.14.6_windows_amd64.zip
```

Extract it.

Inside you will find:

```
terraform.exe
```

---

# 10. Adding Terraform to PATH

Move the extracted `terraform.exe` to a folder and add that folder to:

```
PATH Environment Variable
```

This allows Terraform to run from **any location in PowerShell**.

Example command to verify installation:

```
terraform --help
```

If the command works, Terraform is successfully installed.

---

# 11. Working in PowerShell

Open **PowerShell** and navigate to your project folder.

Example:

```
cd DevOps-Insiders
cd Terraform
cd rg-using-terraform-07-03-2026
```

Now Terraform commands will run inside this folder.

---

# 12. Terraform Documentation

Terraform documentation is extremely important.

Official source:

```
https://registry.terraform.io/
```

This is called the **Terraform Registry**.

It contains:

* Terraform Providers
* Resource definitions
* Example code
* Configuration documentation

---

# 13. Important Learning Philosophy

One important learning rule mentioned:

> We will not memorize Terraform code.

Instead:

1. Search on Google
2. Read official documentation
3. Copy reference code
4. Modify it according to requirement

The goal is to become **documentation-driven engineers**.

---

# 14. Terraform Command (Concept)

Terraform reads `.tf` files and executes them.

Conceptually the command will:

1. Read the Terraform file
2. Understand the resources
3. Create infrastructure in Azure

Example idea:

```
Terraform reads file
→ Terraform connects to Azure
→ Terraform creates resource group
```

---

# 15. Practical Workflow

Complete workflow will look like this:

### Step 1

Create folder structure

### Step 2

Create `.tf` file

### Step 3

Write Terraform configuration

### Step 4

Login to Azure

```
az login
```

### Step 5

Run Terraform commands

Terraform will then create infrastructure automatically.

---

# 16. Key DevOps Habit

A very important mindset for DevOps engineers:

> "Rag Rag me bandh lo – Official documentation ko pad pad ke chithde uda dena hai."

Meaning:

A real DevOps engineer must:

* Read official docs deeply
* Understand tools from source
* Not rely only on tutorials

---

# 17. Daily Revision Plan

Schedule mentioned:

```
Monday to Friday
9:30 PM
Complete Revision
```

Purpose:

* Reinforce Terraform concepts
* Practice commands
* Repeat infrastructure creation

---

# 18. Summary

In this session we learned:

• What Terraform does
• Infrastructure as Code concept
• Folder structure for Terraform projects
• Creating `.tf` files
• Installing Azure CLI
• Logging into Azure
• Installing Terraform
• Using PowerShell
• Using Terraform Registry documentation

This forms the **foundation of Terraform-based Infrastructure Automation**.
