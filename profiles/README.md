# Welcome to the Wakefern Tech GitHub

This is the central landing page for all developers within the **Wakefern Tech** division

Use the resources below to get onboarded and start contributing to projects & applications.

---

## Quick Start

- [Set up an SSH Auth Token](#setting-up-an-ssh-token)

---

<!-- TODO: Populate this section -->

### Setting up an SSH token

> If using a Windows PC, these commands must be run using the Git Bash Terminal Application.

1. **Generate Key Pair:**

   Run the following in your terminal to create a secure Ed25519 key:

   ```bash
   # Replace firstName.lastName@wakefern.com with your wakefern email address
   ssh-keygen -t ed25519 -C "firstName.lastName@wakefern.com"
   ```

2. **Add to SSH Agent:**

   Start the agent and add your new private key:

   ```bash
   # Start Agent
   eval "$(ssh-agent -s)"

   ssh-add ~/.ssh/id_ed25519
   ```

3. **Add Public Key to GitHub:**

   - Copy your public key by opening the `~/.ssh/id_ed25519.pub` file OR

     ```bash
     cat ~/.ssh/id_ed25519.pub
     ```

   - Go to GitHub SSH Settings.
   - Click **New SSH key**, paste your key, and save.

4. **Test Connection:**
   Verify the connection:

   ```bash
   ssh -T git@github.com
   ```

---

_Maintained by the **Wakefern Tech Infrastructure DevOps Team**._

<!-- Found an error? [Open an issue here](https://github.com). -->
