
# We strongly recommend using the required_providers block to set the
# Azure Provider source and version being used

terraform {

  required_providers {
  
    azurerm = {
    
      source  = "hashicorp/azurerm"
      
      version = "=4.70.0"
      
  }
  
  }
    
}

# Configure the Microsoft Azure Provider

provider "azurerm" {

 features {}
 
}

# Create a resource group

resource "azurerm_resource_group" "dilip" {

  name     = "dilip-rg"
  
  location = "West Europe"
  
}

# Create a storage account

resource "azurerm_storage_account" "dilipk" {

  name                     = "storagegold"
  
  resource_group_name      = azurerm_resource_group.dilipk.name
  
  location                 = azurerm_resource_group.dilipk.location
  
  account_tier             = "Standard"
  
  account_replication_type = "GRS"
  
  }
  
