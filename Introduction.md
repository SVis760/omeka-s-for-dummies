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
