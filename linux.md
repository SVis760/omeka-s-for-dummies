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
