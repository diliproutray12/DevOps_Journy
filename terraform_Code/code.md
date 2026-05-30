
# We strongly recommend using the required_providers block to set the
# Azure Provider source and version being used

```hcl
terraform {
  required_providers {
    azurerm = {
      source  = "hashicorp/azurerm"
      version = "4.73.0"
    }
  }
}
```

# Configure the Microsoft Azure Provider

```hcl
provider "azurerm" {
 features {}
 }
```

# Create a resource group (Hard code)

```hcl
resource "azurerm_resource_group" "rg" {
  name     = "dilip-rg"
  location = "West Europe"
}
```
# Create a storage account (explicity)
```hcl
resource "azurerm_storage_account" "dilipk" {
  depends_on               = [azurerm_resource_group.rg]
  name                     = "storagegold"
  resource_group_name      = "dilip-rg"
  location                 = "West Europe"
  account_tier             = "Standard"
  account_replication_type = "GRS"
}
 ```

# Create a storage account (implicity)

```hcl
resource "azurerm_storage_account" "dilipk" {
  name                     = "storagegold"
  resource_group_name      = azurerm_resource_group.dilipk.name
  location                 = azurerm_resource_group.dilipk.location
  account_tier             = "Standard"
  account_replication_type = "GRS"
}
  ```
# Create a Contanier 
```hcl
resource "azurerm_storage_container" "dilipk" {
  name                 = "dilu"
  storage_account_id   = azurerm_storage_account.dilipk.id
  container_acces_type = "private"
}
 ```
# Backend Block
```hcl
backend "azurerm" {
  resource_group_name  = "dilip-rg"
  storage_account_name = "storagegold"
  container_name       = "dilu"
  key                  = "dilip.tfstate"
}
```
# Terraform variables Type1 RG or terraform.tfvars ko variable values file bloti hai.
# main.tf
```hcl
resource "azurerm_resource_group" "name"{
name = var.dilip
location = var.rglocation
}
```
# varieble.tf
```hcl
variable "dilip"{}   
variable "rglocation"{}

(first varieble diclare dilip name then use to main.tf file var.dilip/location=var.rglocation, then assined to terraform.tfvars)

```
# Terraform.tfvars
```hcl
dilip = "rg1"
rglocation  = "centralindia"
```








