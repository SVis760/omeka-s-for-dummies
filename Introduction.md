Omeka S can be installed and run efficiently using Docker containers, which simplifies the setup process by packaging the application with all its dependencies. This method provides a consistent environment across different operating systems, making it easier to install Omeka S on Linux, macOS, and Windows. In this guide, we will walk through the step-by-step process of installing Omeka S using Docker, including the necessary setup for each operating system.

To install Omeka S using Docker, you need to have Docker, MySQL, and Git installed on your system. 

## 1.1 Install Docker
Docker is a platform that allows you to create, deploy, and run applications in containers. Follow these instructions for your operating system:

### Linux
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

### macOS
1. Download and install Docker Desktop for macOS from the [Docker website](https://www.docker.com/products/docker-desktop).
2. Open Docker Desktop and follow the installation instructions.
3. Verify Docker installation by opening a terminal and running:
    ```bash
    docker --version
    ```

### Windows
1. Download Docker Desktop for Windows from the [Docker website](https://www.docker.com/products/docker-desktop).
2. Run the installer and follow the on-screen instructions to set up Docker Desktop.
3. After installation, ensure Docker is running and check the installation with:
    ```bash
    docker --version
    ```



## 1.2 Install MySQL
Omeka S requires a MySQL database. Here's how to install MySQL on different systems:

### Linux
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

### macOS
1. Install MySQL using Homebrew:
    ```bash
    brew install mysql
    ```
2. Start MySQL:
    ```bash
    brew services start mysql
    ```

### Windows
1. Download MySQL Installer from the [official MySQL website](https://dev.mysql.com/downloads/installer/).
2. Run the installer and select "MySQL Server" during the installation process.
3. Follow the on-screen instructions to complete the setup.

## 1.3 Install Git
Git is a powerful version control system that allows you to track changes in your code and collaborate with others. This tutorial will guide you through the basic steps of installing Git, configuring it, and using fundamental Git commands.

### Linux
1. Open a terminal and run:
    ```bash
    sudo apt-get update
    sudo apt-get install git
    ```

### macOS
1. Install Git using Homebrew:
    ```bash
    brew install git
    ```
2. Alternatively, install Xcode Command Line Tools:
    ```bash
    xcode-select --install
    ```

### Windows
1. Download the Git installer from the [official Git website](https://git-scm.com/download/win).
2. Run the installer and follow the default setup instructions.

## 2. Configuring Git

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

