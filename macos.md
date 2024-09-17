To install Omeka S using Docker, you need to have Docker, MySQL, and Git installed on your system. 

## 1.1 Install Docker
Docker is a platform that allows you to create, deploy, and run applications in containers. Follow these instructions for your operating system:

### macOS
1. Download and install Docker Desktop for macOS from the [Docker website](https://www.docker.com/products/docker-desktop).
2. Open Docker Desktop and follow the installation instructions.
3. Verify Docker installation by opening a terminal and running:
    ```bash
    docker --version
    ```

## 1.2 Install MySQL
Omeka S requires a MySQL database. Here's how to install MySQL on different systems:

### macOS
1. Install MySQL using Homebrew:
    ```bash
    brew install mysql
    ```
2. Start MySQL:
    ```bash
    brew services start mysql
    ```

## 1.3 Install Git
Git is a powerful version control system that allows you to track changes in your code and collaborate with others. This tutorial will guide you through the basic steps of installing Git, configuring it, and using fundamental Git commands.


### macOS
1. Install Git using Homebrew:
    ```bash
    brew install git
    ```
2. Alternatively, install Xcode Command Line Tools:
    ```bash
    xcode-select --install
    ```


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
```
