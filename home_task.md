# Home Task - Lab 07

## 1. Environment Variables

- For quick testing, I would use a temporary shell variable because it is available only in the current shell session.
- For a setting only for myself, I would use `~/.bashrc` because it applies to my user account.
- The `.bashrc` file automatically loads these settings when a new Bash shell starts.
- For a setting required by all users, I would use `/etc/environment` because it stores system-wide environment variables.
- These locations provide different levels of availability and persistence.
- Temporary variables are suitable for testing, while the other two locations are useful for persistent settings.

## 2. SSH Key Security

- SSH keys are safer than passwords because they use public-key cryptography for authentication.
- The private key stays on the client machine, while the public key is stored on the server.
- A private key should always be protected with a strong passphrase and proper file permissions.
- If someone steals the private key, they may gain access to servers that trust its corresponding public key.
- In this situation, the stolen key should be revoked by removing its public key from the affected servers.
- A new SSH key pair should then be generated and configured for secure access.
