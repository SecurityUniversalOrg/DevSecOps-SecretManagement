# GitHub SSH Private Key
___
1. Generate a New SSH Key Pair:
   * Run ssh-keygen -t ed25519 -C "your_email@example.com" in your terminal.
   * Follow the prompts to save the key.

2. Add the Public Key to GitHub:
   * Copy the contents of the new .pub file.
   * In GitHub, navigate to Settings > SSH and GPG keys > New SSH key.

3. Update Servers and Services:
   * Replace the old private key in all locations where it is used.

4. Remove the Old SSH Key:
   * Delete the old key from GitHub and any local or remote systems.