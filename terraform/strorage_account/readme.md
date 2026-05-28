resource "azurerm_resource_group" "rg1" {

  name     = "dev-rg"
  
  location = "Central India"
}

resource "azurerm_storage_account" "storage1" {

  name                     = "dilipstorage12345"
  
  resource_group_name      = azurerm_resource_group.rg1.name

  
  location                 = azurerm_resource_group.rg1.location
  
  account_tier             = "Standard"
  
  account_replication_type = "LRS"
}
