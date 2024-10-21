# Viewing GitHub Secret Scanning Findings

---

Once secret scanning is enabled, review the findings regularly:

* Access Secret Scanning Alerts:
  * Go to your repository's Security tab.
  * Select Secret scanning alerts from the sidebar.

* Review Detected Secrets:
  * Browse through the list of detected secrets.
  * Click on individual alerts to see details like the type of secret, file location, and commit history.

* Remediate Detected Secrets:
  * Revoke or Rotate the Secret: Immediately revoke or rotate the exposed secret.
  * Remove the Secret from Code: Delete the secret from the codebase.
  * Commit the Changes: Ensure the removal is committed and pushed to the repository.