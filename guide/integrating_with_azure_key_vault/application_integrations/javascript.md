# JavaScript
___
* Prerequisites:
   * Install packages: npm install @azure/identity @azure/keyvault-secrets

* Sample Code:
```javascript
const { DefaultAzureCredential } = require("@azure/identity");
const { SecretClient } = require("@azure/keyvault-secrets");

const credential = new DefaultAzureCredential();
const vaultName = "<Your-Key-Vault-Name>";
const url = `https://${vaultName}.vault.azure.net`;

const client = new SecretClient(url, credential);

async function getSecret() {
  const secretName = "MySecret";
  const secret = await client.getSecret(secretName);
  console.log(`Secret Value: ${secret.value}`);
}

getSecret();
```
