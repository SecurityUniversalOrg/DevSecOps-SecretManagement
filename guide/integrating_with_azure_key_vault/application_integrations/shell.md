# Shell
___
* Using Azure CLI:
```bash
az keyvault secret show --vault-name <Your-Key-Vault-Name> --name MySecret --query value -o tsv
```