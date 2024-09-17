# Windows Installation Guide for Docker, MySQL and git.

To install Omeka S using Docker, you need to have Docker, MySQL, and Git installed on your system. 

## 1.1 Install Docker
Docker is a platform that allows you to create, deploy, and run applications in containers. Follow these instructions for your operating system:

1. Download Docker Desktop for Windows from the [Docker website](https://www.docker.com/products/docker-desktop).
2. Run the installer and follow the on-screen instructions to set up Docker Desktop.
3. After installation, ensure Docker is running and check the installation with:
    ```bash
    docker --version
    ```

## 1.2 Install MySQL
Omeka S requires a MySQL database. Here's how to install MySQL on different systems:
1. Download MySQL Installer from the [official MySQL website](https://dev.mysql.com/downloads/installer/).
2. Run the installer and select "MySQL Server" during the installation process.
3. Follow the on-screen instructions to complete the setup.

## 1.3 Install Git
Git is a powerful version control system that allows you to track changes in your code and collaborate with others. This tutorial will guide you through the basic steps of installing Git, configuring it, and using fundamental Git commands.

1. Download the Git installer from the [official Git website](https://git-scm.com/download/win).
2. Run the installer and follow the default setup instructions.

## 1.4 Configuring Git

Once Git is installed, configure it with your name and email. This information will be used to track your commits.

1. Set your username:
    ```bash
    git config --global user.name "Your Name"
    ```

2. Set your email:
    ```bash
    git config --global user.email "your.email@example.com"
    ```

You can check your configuration at any time with:
```bash
git config --list
```
