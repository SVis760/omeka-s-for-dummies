# MacOS Installation Guide for Docker, MySQL and git.
To install Omeka S using Docker, you need to have Docker, MySQL, and Git installed on your system. 

## 1.1 Install Docker
Docker is a platform that allows you to create, deploy, and run applications in containers. Follow these instructions for your operating system:

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

Once MySQL is installed and running on your macOS system, you can use the MySQL command-line interface to manage databases and users.
Access MySQL Command Line:

3. Log in to the MySQL shell using the root user:
    ```bash
    mysql -u root -p
    ```
4. Enter the root password when prompted. You should now see the MySQL prompt (`mysql>`).

5. To create a new database, use the following SQL command:
    ```sql
    CREATE DATABASE my_database;
    ```
6. Replace `my_database` with your desired database name.

7. To create a new MySQL user, run:
    ```sql
    CREATE USER 'newuser'@'localhost' IDENTIFIED BY 'password';
    ```
8. Replace `newuser` with the username and `password` with a strong password.

9. Grant the new user full access to the database you created:
    ```sql
    GRANT ALL PRIVILEGES ON my_database.* TO 'newuser'@'localhost';
    ```
10. Apply the changes:
    ```sql
    FLUSH PRIVILEGES;
    ```
11. To exit the MySQL shell, type:
    ```sql
    EXIT;
    ```
After setting up MySQL, test the installation to ensure it's working correctly.
Open Terminal.

12. Log in using the root user:
    ```bash
    mysql -u root -p
    ```
13. Enter the root password when prompted.

14. To list all databases in MySQL, use:
    ```sql
    SHOW DATABASES;
    ```
15. You should see a list of databases, including the one you created (`my_database`).

16. Verify that the new user has access to the database:
    ```bash
    mysql -u newuser -p
    ```
17. Enter the password for `newuser`.
18. Once logged in, list the databases accessible to this user:
    ```sql
    SHOW DATABASES;
    ```
19. You should see `my_database` listed.

20. Type `EXIT;` to exit the MySQL shell:
    ```sql
    EXIT;
    ```

---

You have now successfully installed, configured, and tested MySQL on macOS. You can use these basic commands to manage your MySQL databases and users.





## 1.3 Install Git
Git is a powerful version control system that allows you to track changes in your code and collaborate with others. This tutorial will guide you through the basic steps of installing Git, configuring it, and using fundamental Git commands.

1. Install Git using Homebrew:
    ```bash
    brew install git
    ```
2. Alternatively, install Xcode Command Line Tools:
    ```bash
    xcode-select --install
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
