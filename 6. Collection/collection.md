# Setup EC2 collections and Authentication

## Install Boto3
``` pip install boto3 ```

## Install aws collection
``` ansible-galaxy collection install amazon.aws ```

## Setup Vault
1. Create a password for the vault
``` openssl rand -base64 2048 > vault.pass ```

2. Add your AWS credentials using the below vault command
``` ansible-vault create group_vars/all/pass.yml --vault-password-file vault.pass ```
