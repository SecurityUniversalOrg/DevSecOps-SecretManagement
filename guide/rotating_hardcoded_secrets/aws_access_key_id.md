# AWS Access Key ID
AWS Access Keys (Access Key ID and Secret Access Key) are used to sign programmatic requests to AWS services. Rotating these keys regularly and removing hardcoded keys from code repositories are crucial steps in maintaining the security of your AWS environment. This section provides a comprehensive guide on how to rotate AWS Access Keys securely.
___
## Step 1: Create New Access Keys
1. Log in to the AWS Management Console

* Go to the AWS Management Console.
* Enter your AWS account credentials to log in.
* Ensure you are logged in as the user whose access keys you wish to rotate or as an administrator with permissions to manage IAM users.

2. Navigate to the IAM Service

* From the AWS Console homepage, click on Services at the top of the page.
* Under Security, Identity, & Compliance, select IAM (Identity and Access Management).

3. Select the User

* In the IAM Dashboard, click on Users in the left navigation pane.
* Find and click on the username for which you want to create new access keys.
* Tip: You can use the search bar to quickly locate the user.

4. Create New Access Keys

* Go to the Security credentials tab for the selected user.
* Scroll down to the Access keys section.
* Click on the Create access key button.
* If prompted with a security warning, read the message and click Proceed if you agree.

5. Download or Copy the New Access Keys

* The new Access Key ID and Secret Access Key will be displayed.
* Click Download .csv file to save the keys to a secure location.
* Alternatively, click Show to display the Secret Access Key and manually copy both keys.
* Important: This is the only time the Secret Access Key will be available. If you lose it, you will need to generate new access keys.
* Security Reminder: Store the keys in a secure location, such as a password manager or encrypted file. Do not share them via email or store them in plain text files.

## Step 2: Deactivate and Delete Old Access Keys
1. Deactivate the Old Access Keys

* In the IAM console, navigate back to the Access keys section for the user.
* Locate the old access keys (they will have a different Access Key ID from the new ones).
* Click on the Deactivate button (it looks like a pause icon) next to the old access keys.
* Confirm Deactivation: Read the warning and confirm you want to deactivate the keys.
* Note: Deactivating the keys first allows you to ensure that no services are still using them before deletion.

2. Monitor for Any Issues

* Monitor Applications and Services:
    * Ensure that deactivating the old keys does not cause service disruptions.
* Check CloudWatch Logs and Metrics:
    * Look for any failed authentication attempts or errors.

3. Delete the Old Access Keys

* Once confident that the old keys are no longer in use:
    * In the IAM console, click on the Delete button (trash can icon) next to the deactivated access keys.
    * Confirm Deletion: A prompt will ask you to confirm; proceed with deletion.
* Security Benefit: Deleting ensures the keys cannot be reactivated or misused.