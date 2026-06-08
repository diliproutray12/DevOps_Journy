# 📘 Terraform + VS Code Setup Notes

## 🧠 1. Current Progress (Kahani Ab Tak)

You have already completed:

* ✅ Installed **VS Code**
* ✅ Installed **Terraform Extension** in VS Code
* ✅ Installed **Azure CLI (az cli)**
* ✅ Logged in using:

  ```
  az login
  ```
* ✅ Created a folder and opened it in VS Code
* ✅ Created a Terraform file (e.g., `rg.tf`)
* ✅ Installed **Terraform**

---

## ☁️ 2. What is Terraform?

* Terraform is an **Infrastructure as Code (IaC)** tool.
* It is used to create and manage infrastructure on multiple cloud providers.

### 🌍 Supported Clouds:

* Azure (~300 resources)
* AWS (~500 resources)
* GCP (~250 resources)

---

## ⚙️ 3. Terraform Components

### 3.1 Terraform Executable

* File: `terraform.exe` (~98 MB)
* This is the main engine.

---

### 3.2 Providers (Very Important 🔥)

* Terraform **cannot directly talk to cloud**
* It needs a **Provider (Dalla 😄)**

👉 Example:

* Azure → `azurerm`
* AWS → `aws`
* GCP → `google`

💡 Think of provider as:

> “Bridge between Terraform and Cloud”

---

## 📦 4. Installing Providers

Providers are installed using:

```
terraform init
```

### Commands Flow:

1. `terraform init` → installs providers
2. `terraform plan` → shows execution plan
3. `terraform apply` → creates resources

---

## 💻 5. Terraform Coding Language

### ❌ Traditional Languages:

* C, C++, Java, Python → **Line by Line**

### ✅ Terraform Language:

* HCL (HashiCorp Configuration Language)
* Works **Block by Block**

---

## 🧱 6. Understanding Blocks

### Block Structure:

```
block_name {
  argument = value
}
```

---

### Types of Blocks:

#### 1. Simple Block

```
block_name {
}
```

#### 2. Single Label Block

```
block_name "name" {
}
```

#### 3. Double Label Block

```
block_name "type" "name" {
}
```

---

### 🧩 Example:

```
resource "azurerm_resource_group" "example" {
  name     = "my-rg"
  location = "East US"
}
```

---

## 🧾 7. Brackets in Terraform

| Symbol | Name                             |
| ------ | -------------------------------- |
| ()     | Parenthesis                      |
| []     | Square Brackets                  |
| {}     | Curly Braces ✅ (used for blocks) |

⚠️ Important:

```
= {}
```

This is **NOT a block**, it’s an assignment.

---

## 🏗️ 8. Terraform File (.tf)

* Terraform code is written in `.tf` files
* Example:

  ```
  rg.tf
  ```

---

## 📦 9. Important Terraform Blocks

### 9.1 Terraform Block

```
terraform {
  required_providers {
    azurerm = {
      source = "hashicorp/azurerm"
    }
  }
}
```

👉 Purpose:

* Defines required providers

---

### 9.2 Provider Block

```
provider "azurerm" {
  features {}
}
```

👉 Purpose:

* Connect Terraform to Azure

---

### 9.3 Resource Block

```
resource "azurerm_resource_group" "example" {
  name     = "my-rg"
  location = "East US"
}
```

👉 Purpose:

* Creates actual cloud resources

---

## 🧩 10. Arguments

* Arguments are **key-value pairs inside blocks**

Example:

```
name = "my-rg"
```

---

### Types of Arguments:

* ✅ Required
* 🔹 Optional

💡 Note:

> Arguments can also contain **nested blocks**

---

## 🔍 11. How to Learn Any Block?

👉 Rule:

> “Google + Documentation = Mastery”

Example:

* Search: `terraform azurerm_resource_group`
* Read official docs

---

## 🔁 12. Key Concept Recap

* Terraform works **block by block**
* Blocks connect → form full configuration
* Every block contains **arguments**
* Providers are mandatory to connect to cloud
* `.tf` files store Terraform code

---

## 🚀 13. Complete Flow

1. Write `.tf` file
2. Run:

   ```
   terraform init
   ```
3. Run:

   ```
   terraform plan
   ```
4. Run:

   ```
   terraform apply
   ```

---

## 💡 Final Understanding

* Terraform = Engine (`terraform.exe`)
* Provider = Cloud connector
* HCL = Language
* Blocks = Building units
* Arguments = Configuration inside blocks
