# Self-Service Guide to Identifying and Mitigating Hardcoded Secrets

Welcome to the self-service guide designed to help developers identify and mitigate hardcoded secrets in their application and infrastructure code. This guide provides comprehensive steps to enhance your application's security posture by eliminating hardcoded secrets and integrating secure secret management solutions.

---

## Table of Contents
* Identifying Hardcoded Secrets
  * Setting up GitHub Secret Scanning
  * Viewing GitHub Secret Scanning Findings

* Rotating Hardcoded Keys
  * GitHub App Installation Access Token 
  * GitHub Personal Access Token
  * Google API Key
  * Atlassian API Token
  * Google Cloud Service Account Credentials
  * Azure Active Directory Application Secret
  * AWS Secret Access Key
  * AWS Access Key ID
  * Azure Storage Account Access Key
  * Google Cloud Storage Access Key Secret
  * Slack Incoming Webhook URL
  * Databricks Access Token
  * GitHub SSH Private Key
  * Twilio Account String SID

* Integrating with Azure Key Vault
  * Setting Up Azure Key Vault
  * Configuring and Managing Azure Key Vault
  * Application Integrations
    * Java
    * JavaScript
    * Python
    * C#
    * Shell
  * Infrastructure Integrations
    * Terraform
    * Docker
    * Kubernetes/Helm
  * CI/CD Platform Integrations
    * Jenkins
    * GitHub Actions