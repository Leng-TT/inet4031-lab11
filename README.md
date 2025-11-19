# INET4031 - Lab 11 Puppet
## User and Group Management
The file server_users_groups.pp controls which users and groups should exist on the server.
Puppet creates four users (user04, user05, user06, user07) and two groups (group01, group02).
Each user is configured with:
- A hashed password
- A login shell
- The correct group assignments
- A managed home directory
## LAMP Stack Server Role
The file lamp_stack_server.pp defines a basic LAMP Stack role using Puppet.
Puppet installs and manages the packages needed for:
- Apache2 (web server)
- PHP and required PHP modules
- MariaDB (MySQL server)
- A PHP test page (phpinfo.php) copied into /var/www/html/
The manifest also ensures that the Apache and MariaDB services are running and enabled after reboot.
Essentially instead of doing it manually, now it is automated with Puppet.
## Purpose
Essentially this repository demonstrates how Puppet can be used to automate:
- User management
- Group management
- Package installation
- Service configuration
- Web server setup
- Database server setup
By treating infrastructure as code, configuration becomes consistent, repeatable, and version-controlled.

