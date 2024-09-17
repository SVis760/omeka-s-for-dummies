# How to run an Omeka-S Docker image on MacOS.
For this guide we will be using the following repository from the Ghent University: https://github.com/GhentCDH/Omeka-S-Docker.git

1. In your system, open a terminal. You can do this by pressing Cmd + Space to open Spotlight, typing "Terminal," and pressing Enter.
2. Navigate to the Applications Folder
In this folder the Omeka-S-Docker folder will be placed, if you rather place the folder somewhere else then navigate to that folder. I recommend not placing it in a Download folder.
To navigate to the Applications folder using the terminal, use the cd command:
```bash
cd /Applications
```

3. Verify Your Current Directory
To ensure that you are in the correct directory, use the pwd command:
```bash
pwd
```

4. Clone the Git Repository
```bash
git clone https://github.com/GhentCDH/Omeka-S-Docker.git
```
This command will create a new folder named Omeka-S-Docker inside the Applications directory and copy all files from the repository into this folder.
5. To verify that the repository has been cloned successfully, list the contents of the Applications directory:
```bash
ls
```
6. You should see a directory named Omeka-S-Docker in the output. Now you can navigate to this folder:
```bash
cd Omeka-S-Docker
```
Now we will closely follow the instruction from the repo with some extra clarification steps and notes.

Before any further step, the configuration files first need to be set up. This is because Omeka-S uses the MySQL login credentials to connect to the database. In the Omeka-S-Docker folder there is an example.env file, which is an example of how to set it up. 

The first step forward is to make a copy of the example.env file to .env (this will be how the new file is called) and update the values as needed:
```bash
# MySQL/MariaDB configuration
MYSQL_ROOT_PASSWORD=your_root_password
MYSQL_DATABASE=omeka_db
MYSQL_USER=omeka_usr
MYSQL_PASSWORD=your_password
MYSQL_HOST=omeka-db

# Omeka-S SMTP configuration
# For more details, see: https://docs.laminas.dev/laminas-mail/transport/smtp-options/
EMAIL_HOST=smtp.example.com
EMAIL_PORT=587
EMAIL_USER=your_email_user
EMAIL_PASSWORD=your_email_password
EMAIL_CONNECTION_TYPE=tls
HOST_NAME=example.com
```
The variables were set up during the installation process of MySQL, see [MacOS Installation Guide for Docker, MySQL and git](macos.md), step 5-8.
