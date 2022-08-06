## Creating an SSH Key

1. Check for existing SSH keys in your ~/.ssh folder by running this command:
```ls -al ~/.ssh```
If there are no results printed (or see no directroy matching that name) then you
don't have any keys, if there are results then you can see which keys you already have generated.
2. Generate a new SSH key:
    - Run the command, substituting your GitHub email address
    ```ssh-keygen -t ed25519 -C "your_email@example.com"``` 
    - When prompted for a file to save the key just hit enter for the default location
    - Either enter a password or hit enter to have no password

## Adding SSH Key to GitHub

1. Copy the contents of the SSH key file by using the following command:
```pbcopy < ~./ssh/name_of_ssh_file.pub```
2. Navigate to settings on GitHub by clicking on your profile and then clicking settings
3. Click on Access in the sidebar
4. Click SSH and GPG keys
5. Click "New SSH Key" or "Add SSH Key"
6. In the title field give the key a title (ie. Your_Name_MacBook_Pro)
7. Paste your key into the "Key" field
8. Click "Add SSH Key"
