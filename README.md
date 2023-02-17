                        ** This Project is still in Development **

Description: 

Creating a high availability website. RDS is my SQL and multi-AZ will be enabled. Website used is wordpress and apache webserver and also created writable and readable nodes.
If Admins hit the website, they will be directed to the writable nodes and users to the readable nodes using Route 53. 
Content of website will be synced with both buckets
One S3 bucket will used as a backup if website goes down. Crontab will be used to upload content every minute.
Content Network Delivery( Cloudfront) isused to get the user to access the media stored on the S3 bucket for any incoming request

Pre-requisites
AWS CLI installed
IAM user with programmatic access and configured on CLI
IAM role for services to access other services
Wordpress installed on LAMP

![AWS project with database and s3 oct 8](https://user-images.githubusercontent.com/94655040/219560035-c6a2db8c-3c88-43f7-88b1-9e4d83a647ce.PNG)


