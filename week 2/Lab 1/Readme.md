Working with IAM management console

Tasks

1. Login to your root account
2. Create an IAM group with S3 read only acess (S3 support).
3. Create an IAM group with EC2 read only acess (EC2 support)
4. Create an IAM group with EC2 full access (EC2 admin)
5. Create 3 IAM users and add to the each group above as descibe below:


user      group          permissions
user1     EC2 support     Read-Only access to Amazon EC2
user2     S3 support      Read-Only access to Amazon S3
user3     EC2 admin       Full access to Amazon EC2 instances

6. Test your design

7. Perform clean up operations


Replicate the process above forthe Schulltech organization described below:


|user               |group        |  permissions

adminstaff - -  EC2 support ---        | Read-Only access to Amazon EC2

|Techstaff          |S3 support           |Full access to S3

|ITexpert           |EC2/SDK admin        |full access to EC2 and SDK

|financialmanager   | billingcontrol      |Billing Full Access  

|financeuser        |billinguser          |Billing view access



https://docs.aws.amazon.com/IAM/latest/UserGuide/tutorial_users-self-manage-mfa-and-creds.html


Submitting the assignment

1. Take a screenshot of each completed step
2. Attach the screenshot to an output directory
3. Push the updated repository to your own git account



## Solution

### User Group
1. EC2 support
![EC2 support](screenshots/groups/EC2%20READ%20ONLY%20GROUP.PNG)


2. S3 support 
![S3 support](screenshots/groups/S3SUPPORT.PNG)


3. EC2/SDK admin
![EC2/SDK admin](screenshots/groups/EC2SDK.PNG)


4. billingcontrol
![billingcontrol](screenshots/groups/BILLINGCONTROL.PNG)


5. billinguser
![billinguser](screenshots/groups/BILLINGUSER.PNG)


### Users
![Users](screenshots/users/all%20users.PNG)


### Test
1. Adminstaff
![Adminstaff](screenshots/design%20test/adminstaff_create%20instance.PNG)


2. Techstaff
![Techstaff](screenshots/design%20test/techstaff-create%20bucket.PNG)


3. ITexpert
![ITexpert](screenshots/design%20test/ITexpert-createEC2.PNG)


4. financialmanager
![financemanager](screenshots/design%20test/financemanager-billingaccess.PNG)


5. financeuser
![financeuser](screenshots/design%20test/financeuser-billing.PNG)


