# Self-Service Guide to Identifying and Mitigating Hardcoded Secrets

Welcome to the self-service guide designed to help developers identify and mitigate hardcoded secrets in their application and infrastructure code. This guide provides comprehensive steps to enhance your application's security posture by eliminating hardcoded secrets and integrating secure secret management solutions.

---

## Table of Contents
* [Identifying Hardcoded Secrets](guide/identifying_hardcoded_secrets/README.md)
  * [Setting up GitHub Secret Scanning](guide/identifying_hardcoded_secrets/setting_up_github_secret_scanning.md)
  * [Viewing GitHub Secret Scanning Findings](guide/identifying_hardcoded_secrets/viewing_github_secret_scanning_findings.md)

* [Rotating Hardcoded Keys](guide/rotating_hardcoded_secrets/README.md)
  * [GitHub App Installation Access Token ](guide/rotating_hardcoded_secrets/github_app_installation_access_token.md)
  * [GitHub Personal Access Token](guide/rotating_hardcoded_secrets/github_personal_access_token.md)
  * [Google API Key](guide/rotating_hardcoded_secrets/google_api_key.md)
  * [Atlassian API Token](guide/rotating_hardcoded_secrets/atlassian_api_token.md)
  * [Google Cloud Service Account Credentials](guide/rotating_hardcoded_secrets/google_cloud_service_account_credentials.md)
  * [Azure Active Directory Application Secret](guide/rotating_hardcoded_secrets/azure_active_directory_application_secret.md)
  * [AWS Secret Access Key](guide/rotating_hardcoded_secrets/aws_secret_access_key.md)
  * [AWS Access Key ID](guide/rotating_hardcoded_secrets/aws_access_key_id.md)
  * [Azure Storage Account Access Key](guide/rotating_hardcoded_secrets/azure_storage_account_access_key.md)
  * [Google Cloud Storage Access Key Secret](guide/rotating_hardcoded_secrets/google_cloud_storage_access_key_secret.md)
  * [Slack Incoming Webhook URL](guide/rotating_hardcoded_secrets/slack_incoming_webhook_url.md)
  * [Databricks Access Token](guide/rotating_hardcoded_secrets/databricks_access_token.md)
  * [GitHub SSH Private Key](guide/rotating_hardcoded_secrets/github_ssh_private_key.md)
  * [Twilio Account String SID](guide/rotating_hardcoded_secrets/twilio_account_string_sid.md)

* [Integrating with Azure Key Vault](guide/integrating_with_azure_key_vault/README.md)
  * [Security Best Practices and Checklist](guide/integrating_with_azure_key_vault/security_guide.md)
  * [Setting Up Azure Key Vault](guide/integrating_with_azure_key_vault/setting_up_azure_key_vault.md)
  * [Configuring and Managing Azure Key Vault](guide/integrating_with_azure_key_vault/configuring_and_managing_azure_key_vault.md)
  * [Application Integrations](guide/integrating_with_azure_key_vault/application_integrations/README.md)
    * [Java](guide/integrating_with_azure_key_vault/application_integrations/java.md)
    * [JavaScript](guide/integrating_with_azure_key_vault/application_integrations/javascript.md)
    * [Python](guide/integrating_with_azure_key_vault/application_integrations/python.md)
    * [C#](guide/integrating_with_azure_key_vault/application_integrations/c_sharp.md)
    * [Shell](guide/integrating_with_azure_key_vault/application_integrations/shell.md)
  * [Infrastructure Integrations](guide/integrating_with_azure_key_vault/infrastructure_integrations/README.md)
    * [Terraform](guide/integrating_with_azure_key_vault/infrastructure_integrations/terraform.md)
    * [Docker](guide/integrating_with_azure_key_vault/infrastructure_integrations/docker.md)
    * [Kubernetes/Helm](guide/integrating_with_azure_key_vault/infrastructure_integrations/kubernetes.md)
  * [CI/CD Platform Integrations](guide/integrating_with_azure_key_vault/cicd_platform_integrations/README.md)
    * [Jenkins](guide/integrating_with_azure_key_vault/cicd_platform_integrations/jenkins.md)
    * [GitHub Actions](guide/integrating_with_azure_key_vault/cicd_platform_integrations/github_actions.md)