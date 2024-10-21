# Terraform
___
* Prerequisites:
   * Install the AzureRM provider.

* Sample Configuration:
```hcl
provider "azurerm" {
  features = {}
}

data "azurerm_key_vault_secret" "example" {
  name         = "MySecret"
  key_vault_id = azurerm_key_vault.example.id
}

resource "azurerm_virtual_machine" "example" {
  # ...
  os_profile_linux_config {
    disable_password_authentication = false
    admin_password                  = data.azurerm_key_vault_secret.example.value
  }
}
```