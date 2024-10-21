# C#    
___
* Prerequisites:
   * Install NuGet packages: Azure.Identity and Azure.Security.KeyVault.Secrets

* Sample Code:
```csharp
using System;
using Azure.Identity;
using Azure.Security.KeyVault.Secrets;

class Program
{
    static void Main(string[] args)
    {
        var kvUri = "https://<Your-Key-Vault-Name>.vault.azure.net/";
        var client = new SecretClient(new Uri(kvUri), new DefaultAzureCredential());

        KeyVaultSecret secret = client.GetSecret("MySecret");
        Console.WriteLine($"Secret Value: {secret.Value}");
    }
}
 ```