
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
  name = "my-rg"
  location = "West Europe"
}
```

# Create a storage account

```hcl
resource "azurerm_storage_account" "dilipk" {
 name                     = "storagegold"
 resource_group_name      = azurerm_resource_group.dilipk.name
 location                 = azurerm_resource_group.dilipk.location
  account_tier             = "Standard"
  account_replication_type = "GRS"
  }
  ```
