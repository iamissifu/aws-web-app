Connect A Web App with Amazon Aurora
Project Overview
This project demonstrates how to connect a web application to an Amazon Aurora database. Aurora is a fully managed relational database service that offers high performance, scalability, reliability, compatibility, and cost-effectiveness, making it ideal for handling demanding workloads such as online transaction processing.

Author
Sibdou Ibrahim Issifu
AmaliTech AWS re/Start

Table of Contents
Project Description
Requirements
Installation
Connecting to Amazon Aurora
Testing the Web Application
Project Duration
Project Description
This project involves creating a web app that connects to an Amazon Aurora database, querying data, and confirming connectivity. The web app is hosted on an EC2 instance, and the database connection is handled using PHP and MySQL.

Requirements
To run this project, you will need:

Apache web server
PHP
MySQL or MariaDB
Amazon EC2 instance
Amazon Aurora database
Installation
Set up the web server and database:
Install Apache, PHP, and MariaDB using the following command:

bash
Copy code
sudo dnf install -y httpd php php-mysqli mariadb105  
Connect to your EC2 instance:
Use the following SSH command to connect to your EC2 instance:

bash
Copy code
ssh -i NextWorkAuroraApp.pem ec2-user@<ec2-instance-ip-address>  
Create a 'dbinfo' file:
Store your EC2 instance's connection details to the Amazon Aurora database in a dbinfo file.

Connecting to Amazon Aurora
Configure the connection details:
Update your PHP script to include the database connection details. These can be stored in a separate dbinfo.php file for security and reusability.

SSH into your instance:
Once again, SSH into your EC2 instance using the provided key:

bash
Copy code
ssh -i NextWorkAuroraApp.pem ec2-user@<ec2-instance-ip-address>  
Testing the Web Application
Upgrade the web app:
Create a PHP file that allows querying the database and retrieving data from Amazon Aurora.

Test the connection:
Use the MySQL CLI to ensure that the web app is correctly connected to the database.

Verify results:
Access the database and confirm the query results to ensure the web app functions as expected.

Project Duration
The project took approximately 2 hours to complete.
