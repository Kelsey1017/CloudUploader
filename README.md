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
