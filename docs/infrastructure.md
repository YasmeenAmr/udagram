### Infrasturcture
We used main 3 services in AWS 


1- RDS :
        Creating database for our udagram app.

 steps:
       1-Click on create database button
       2-Select standard create
       3-Select postgresSql
       4-Choose 12.8-R1 version
       5-Select Free tier 
       6-add password for database-1
       7-Choose db.t2.micro in DB instance class
       8-Uncheck Enable storage autoscalling
       9-Select yes in public access
       10-Select Create new for creating new VPC security group 
       11-Create name for the new group 
       12-in Additional configuration -> add "udagram" in initial database name field
       13-click on create database 
       14-Changing the POSTGRES_HOST ,POSTGRES_USERNAME,POSTGRES_PASSWORD and POSTGRES_DB values in .env file with the new values.


2-S3:
     Storing files and deploying front-end of our udagram app.

steps:
     1-Click on Create bucket 
     2-Create bucket name
     3-Uncheck Block all public access
     4-Select Disable for server-side encryption
     5-Select Disable for Object lock
     6-Click on Create bucket
     7-Click on bucket which you created then choose properties
     8-Scroll down till Static website hosting and click on Edit
     9-Select Enable in Static website hosting,index.html in index document and click on save changes
     10-Then choose permission to make bucket public access
     11-Scroll down till Bucket policy and click on edit
     12-add this policy
     {
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::buc-udagram/*"
        }
    ]
}
    13-then choose Objects to uploade files of website
    14-Uploading www files
    15-In properties you will find the URL-> http://buc-udagram.s3-website-us-east-1.amazonaws.com



3-EB:
    Deploying udagram-api on server

steps:
     1-Open cmd on you device and run aws configure 
     2-Set AWS Access Key ID,AWS Secret Access Key,region and output formate
     3-Open udagram-api in terminal 
     4-Run eb init -> create elasticbeanstalk configration file
     5-Run rb create -> create environment 
     6-Run npm run deploying -> to use udagram-api-dev environment and eb depoly to deploy our application 


