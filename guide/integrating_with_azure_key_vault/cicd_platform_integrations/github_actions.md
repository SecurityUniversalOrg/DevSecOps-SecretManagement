# GitHub Actions
___
* Set Up Azure Login:
   * Store Azure credentials in GitHub Secrets.

* Sample Workflow:
```yaml
name: Build and Deploy

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: azure/login@v1
        with:
          creds: ${{ secrets.AZURE_CREDENTIALS }}
      - name: Get Secret from Key Vault
        run: |
          az keyvault secret show --vault-name <Your-Key-Vault-Name> --name MySecret --query value -o tsv
```