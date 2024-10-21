# Python
___
* Prerequisites:
   * Install packages: pip install azure-identity azure-keyvault-secrets

* Sample Code:
```python
from azure.identity import DefaultAzureCredential
from azure.keyvault.secrets import SecretClient

credential = DefaultAzureCredential()
vault_url = "https://<Your-Key-Vault-Name>.vault.azure.net/"

client = SecretClient(vault_url=vault_url, credential=credential)
secret = client.get_secret("MySecret")
print(f"Secret Value: {secret.value}")
```