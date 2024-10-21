# Java

* Prerequisites:
   * Add the Azure Key Vault and Azure Identity libraries to your project dependencies.

* Sample Code:
```java
import com.azure.identity.DefaultAzureCredentialBuilder;
import com.azure.security.keyvault.secrets.SecretClient;
import com.azure.security.keyvault.secrets.SecretClientBuilder;

public class KeyVaultExample {
    public static void main(String[] args) {
        SecretClient secretClient = new SecretClientBuilder()
            .vaultUrl("https://<Your-Key-Vault-Name>.vault.azure.net/")
            .credential(new DefaultAzureCredentialBuilder().build())
            .buildClient();

        String secretValue = secretClient.getSecret("MySecret").getValue();
        System.out.println("Secret Value: " + secretValue);
    }
}
```