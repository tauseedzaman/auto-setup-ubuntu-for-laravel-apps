# Server Setup Script for Laravel Apps

This script automates the setup of a web server environment with Apache, MySQL (or MariaDB), and PHP. It also configures a MySQL database and installs necessary PHP extensions.

## Prerequisites

- A Unix-based operating system (e.g., Ubuntu)
- Root or sudo privileges

## Script Overview

This script performs the following tasks:

1. Updates the package list and upgrades installed packages.
2. Installs Apache, MySQL (or MariaDB), and PHP.
3. Configures Apache to enable `mod_rewrite`.
4. Installs and secures MySQL server.
5. Creates a MySQL database and user with specified credentials.
6. Installs Composer and necessary PHP extensions.
7. Restarts Apache to apply changes.

## How to Run

1. **Download or copy the script to your server.**
2. **Run the script with root or sudo privileges:**
   ```sh
   sudo bash setup_server.sh
   ```

## Database Configuration

The script includes default database configuration values:

```sh
DB_HOST="127.0.0.1"
DB_PORT="3306"
DB_NAME="dbname"
DB_USER="dbname_user"
DB_PASS="dbname_pass"
```

You can modify these values within the script to match your desired database configuration.

## Important Notes

- Ensure the script is run in a secure environment, as it involves setting up and securing a database.
- Verify that the required PHP extensions (`php-xml` and `php-gd`) are available for your PHP version.
