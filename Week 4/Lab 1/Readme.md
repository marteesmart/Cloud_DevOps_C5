
# Install a LAMP web server on Amazon Linux
Tasks:

1. Prepare the LAMP server
2. Test your LAMP server
3. Secure the database server
4. Install phpMyAdmin


Guide: 

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/install-LAMP.html

Grading tip: Screenshot major script outputs and upload with your step by step answer


## Solution

1. Launch EC2 Instance
![Launch LAMP server](screenshots/4.1.1.PNG)


2. Install Apache,Database(MariaDB),php
![Install AMP](screenshots/4.1.2.PNG)


    ![Install AMP 2](screenshots/4.1.2.2.PNG)


3. Start Apache
![Start Apache](screenshots/4.1.3.PNG)


4. Add ec2-user to group,grant permission to group and change ownership 
![access](screenshots/4.1.4.PNG)


    echo "phpinfo()" and verify
    ![access 2](screenshots/4.1.4.2.PNG)


5. Secure the database server
![secure DB](screenshots/4.1.5.PNG)


6. Install PHP Mbstring extension and phpMyAdmin
![install phpmyadmin](screenshots/4.1.6.PNG)


7. Verify Access to admin tool and Database
![verify phpmyadmin](screenshots/4.1.7.PNG)



