# Atlassian API Token
Atlassian API Tokens are used for authentication when integrating with Atlassian Cloud products such as Jira Cloud, Confluence Cloud, Bitbucket Cloud, and others. Rotating these tokens is crucial to maintain security, especially when they are hardcoded in code repositories or shared among team members. This section provides a comprehensive guide on how to rotate Atlassian API Tokens securely.
___

## Step 1: Generate a New API Token

1. Access the Atlassian API Tokens Page:

* Navigate to the Atlassian account management page.
* Log in with your Atlassian account credentials if prompted.
* Ensure that you are accessing the account associated with the API token you wish to rotate.

2. Create a New API Token:

* Click on the "**Create API token**" button.
* In the dialog that appears, provide a **descriptive label** for the new token. This helps in identifying the token later, especially if you have multiple tokens.
   * **Example**: `Jira Integration for Project Alpha`
* Click "**Create**" to generate the new token.

3. Copy and Securely Store the Token:

* The new API token will be displayed **only once** after creation.
* Click "**Copy to clipboard**" to copy the token.
* **Important**: Securely store the token in a safe location, such as a password manager or encrypted storage.
   * Do **not** store the token in plain text files or share it via unsecured channels.
* If the token is lost or not copied at this point, you will need to generate a new one.


## Step 2: Revoke the Old Token

1. Delete the Old API Token:

* Return to the Atlassian API tokens page.
* Locate the old token in the list. Use the label to identify it.
* Click the "Delete" button (trash can icon) next to the token.
* Confirm the deletion when prompted.

2. Verify Revocation:

* Any systems or applications still using the old token should now fail to authenticate.
* Monitor logs and alerts to ensure there are no unintended service disruptions.

3. Monitor for Unauthorized Access:

* Keep an eye on access logs for any attempts to use the revoked token.
* Investigate any suspicious activities.

