# FlaskLogReg
Login and Registration Page using Flask and MySQL

PROJECT SETUP:

Step1:- Create a Virtual Environment
        py -3 -m venv venv

Step2:- Activate the environment
        venv\Scripts\activate

Step3:- Install Flask and MySQL Connector
        pip install Flask flask-mysqldb

Step4:- Set Up MySQL Database
        4.1: Open MySQL Workbench and open MySQL Connection 'Local instance MYSQL80' (Refresh if not available at first) and enter the password or run the following              command in the terminal and enter password when prompted.
             mysql -u root -p
        4.2: Create the Database "FlaskLogin" by executing the following SQL command
             CREATE DATABASE FlaskLogin DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci;
        4.3: Select 'FlaskLogin' Database from the schema and Create the "accounts" table executing this SQL commands
             USE FlaskLogin;
             CREATE TABLE accounts (
                id INT NOT NULL AUTO_INCREMENT,
                username VARCHAR(50) NOT NULL,
                password VARCHAR(255) NOT NULL,
                email VARCHAR(100) NOT NULL,
                PRIMARY KEY (id)
             ) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8mb4;

![Project Structure](https://github.com/user-attachments/assets/70404ca9-2022-4a02-ba79-f9b3e2d47086)
