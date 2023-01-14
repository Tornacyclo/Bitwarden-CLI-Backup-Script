# Bitwarden-CLI-Backup-Script
This script is designed to automate the process of backing up your Bitwarden vault using the command line interface (CLI). It includes the following steps:

- Download and install the Bitwarden CLI
- Set environment variables for the client ID and secret
- Set a password variable
- Log in and unlock the vault using the password
- Export the vault to an encrypted JSON file

# Prerequisites

- A Bitwarden account with a vault that you want to back up
- A client ID and secret for the Bitwarden CLI (can be obtained from the Bitwarden settings page)
- A password for the Bitwarden vault

# Usage

- Download the script and make it executable
```console
wget https://raw.githubusercontent.com/username/repository/branch/bitwarden_backup.sh
chmod +x bitwarden_backup.sh
```
- Edit the script and replace the placeholders for the client ID, client secret, and password with your actual values
- Run the script
```console
./bitwarden_backup.sh
```

# Advanced usage

You can specify the location where the backup file will be saved by editing the --output flag in the bw export command in the script.

You can also specify the format of the backup file. This script uses encrypted JSON, but you can also use unencrypted JSON or CSV.

# Note

- Make sure the path you are using in the --output flag is existing path.
- Make sure you give the execute permissions to the script before running it.
- Before running the script make sure that you have the latest version of the Bitwarden CLI.
- Also, you can add a cron job to automate the process of backing up your vault.

# Conclusion

This script is a simple and efficient way to automate the process of backing up your Bitwarden vault using the CLI. With a few modifications, it can be customized to suit your specific needs.
