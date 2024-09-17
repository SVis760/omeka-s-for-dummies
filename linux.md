# Installation guide for Docker, MySQL and git for Linux-based distributions.

## 1.1 Install Docker
Docker is a platform that allows you to create, deploy, and run applications in containers. Follow these instructions for your operating system:

1. Update your package list and install Docker:
    ```bash
    sudo apt-get update
    sudo apt-get install docker.io
    ```
2. Start Docker and enable it to start on boot:
    ```bash
    sudo systemctl start docker
    sudo systemctl enable docker
    ```
3. Verify Docker installation:
    ```bash
    docker --version
    ```

## 1.2 Install MySQL
Omeka S requires a MySQL database. Here's how to install MySQL on different systems:

1. Install MySQL server:
    ```bash
    sudo apt-get install mysql-server
    ```
2. Secure the MySQL installation:
    ```bash
    sudo mysql_secure_installation
    ```
3. Start MySQL and ensure it runs on startup:
    ```bash
    sudo systemctl start mysql
    sudo systemctl enable mysql
    ```

## 1.3 Install Git
Git is a powerful version control system that allows you to track changes in your code and collaborate with others. This tutorial will guide you through the basic steps of installing Git, configuring it, and using fundamental Git commands.

1. Open a terminal and run:
    ```bash
    sudo apt-get update
    sudo apt-get install git
    ```

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
