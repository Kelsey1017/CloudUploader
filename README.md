# CloudUploader
The purpose of this project is to smoothly upload files to an AWS S3 bucket using the Bash terminal.

# Prerequisites
- Register or AWS account
- Download and install Git/Bash
- Create IAM user differentiated from root user
- Create security group and role for IAM
- Create SSO for user
- Authenticate SSO through the Git Bash terminal

 # Troubleshooting
 There was issues authenticating a user. There appeared to be a User and Group but that user was not assigned to an account nor the right permissions. This caused and issue in Bash when trying to access an account that was not the root user. After attempting several different options of changing security permissions to the user and creating a different user under the kbadmin profile previously set up through IAM through the root. I was able to assign a user to the kbadmin profile. Bash was able to access the account on autherization. 
Git terminal was limiting authorization and permissions for AWS. I then switched to using Windows terminal, this option was successful.

# New Approach
After completing prerequisites and troubleshooting I proceeded with AWS S3 bucket upload by awscli via terminal. I created a new folder for a static website that held an html file inside for a personalized resume static website. 

# Steps
1. aws configure sso
2. allow permissions
3. create new S3 bucket
4. revise and delete a bucket--create new bucket
5. delete objects in a different bucket, don't need duplicates at this time
6. trial and error via terminal on correct syntax for file uploading into bucket
7. checking progress each step to ensure success
8. project successful
