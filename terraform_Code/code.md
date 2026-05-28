
# We strongly recommend using the required_providers block to set the
# Azure Provider source and version being used

```hcl
terraform {
  required_providers {
  azurerm = {
  source  = "hashicorp/azurerm"
      version = "=4.70.0"
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

# Create a resource group

```hcl
resource "azurerm_resource_group" "rg" {
  name = "dilip-rg"
  location = "West Europe"
}
```
# Create a storage account (explicity)
```hcl
resource "azurerm_storage_account" "dilipk" {
depends_on = [azurerm_resource_group.rg]
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
name                     = "dilu"
storage_account_id = azurerm_storage_account.dilipk.id
container_acces_type = "private"
}
 ```





