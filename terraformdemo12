resource "azurerm_resource_group" "rang" {
  name     = "gitdemo"
  location = "east us"
}

resource "azurerm_storage_account" "str23" {
  name                     = "stname"
  resource_group_name      = azurerm_resource_group.rang.name
  location                 = azurerm_resource_group.rang.location
  account_tier             = "Standard"
  account_replication_type = "GRS"

  tags = {
    environment = "staging"
  }
}
