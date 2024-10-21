# Docker
___
* Using Environment Variables:
   * Fetch secrets from Key Vault and pass them to Docker containers.

* Sample Command:
```bash
docker run -e SECRET_VALUE=$(az keyvault secret show --vault-name <Your-Key-Vault-Name> --name MySecret --query value -o tsv) your-docker-image
```