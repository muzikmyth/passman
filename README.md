# Password Sharing Application

This project contains a user-friendly and powerful php-based password manager with allows an organization or firm to share password credentials with selected users. New multiple users, credentials and modules can be added while editing/modifying. 

# Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Setup](#setup)
- [License](#license)
- [Credits](#credits)


## Features

- This script can be used for following:
    - Create, manage and share passwords.
    - Create, manage and share users.
    - Adding custom CRUD modules.
    - Invite, manage and restrict user registration.
    - Manage permissions.

## Requirements

- Generic web server with following installed:
    - Apache/Nginx Web server
    - PHP v5.5+
    - MySQL/MariaDB
    - GD and cURL Enabled
    - OpenSSL or Let's Encrypt SSL.
    

## Setup

- Open a terminal window and execute one of the following setup sequences :

- Install the required software packages:

      sudo apt install zip

- Download the contents to your desired path:

      sudo git clone https://github.com/muzikmyth/passman.git
      cd passman
      sudo unzip upload.zip

- Alternatively,
    
      sudo wget https://github.com/muzikmyth/passman/raw/master/upload.zip
      sudo unzip upload.zip
        
- We need to create a new database, its user and password. Let's run the following commands:

      sudo mysql -u root -p
    
- Enter your root password which maybe blank by default if you are using MariaDB. After that run the following:

      CREATE USER user@localhost IDENTIFIED BY 'passw0rd';
      CREATE DATABASE passman;
      GRANT ALL PRIVILEGES ON passman.* TO user@localhost IDENTIFIED BY 'passw0rd';
      FLUSH PRIVILEGES;
      quit;

- This would create a user called 'user' with password 'passw0rd' and database name 'passman' and assign grants.

- Now open the url https://website or installed directory https://website/dir/ and if you see installation, then you are good to contiune.
    
- Follow the installation script and you can use the software.

## License

MIT License. Read [LICENSE](LICENSE.md) for details.


## Credits

Developed by [Abhijit Kumar](http://abhijitkrm.site) at Wiregalaxy @ 2016.
