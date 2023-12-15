# Automate-with-Ease-A-Shell-Scripting-Starter 

# Shell scripting 
Shell scripting is a way to automate repetitive tasks or execute a series of commands in a Unix or Linux environment. In our project, the shell script likely serves as a script to be executed by the AWS Lambda function or as part of a broader automation workflow.

# AWS Lambda 
AWS Lambda is a serverless compute service provided by Amazon Web Services (AWS). It allows you to run code without provisioning or managing servers. In your project, AWS Lambda is likely used to execute the shell script in response to an event, such as an S3 bucket event.

# SNS (Simple Notification Service)
SNS is a fully managed messaging service that allows you to send messages or notifications to a distributed set of recipients. In our project, SNS could be used to send notifications or alerts based on the outcomes of your Lambda function execution.

# S3 Bucket 
Amazon S3 (Simple Storage Service) is a scalable object storage service offered by AWS. It allows you to store and retrieve any amount of data at any time. In our project, an S3 bucket is likely used to store files or objects, and events on this bucket trigger the execution of your Lambda function.

# IAM Role
IAM is a service that enables you to manage access to AWS services and resources securely. It provides user authentication and authorization controls. In our project, IAM roles and policies are likely used to grant necessary permissions to your Lambda function, allowing it to interact with other AWS services.


# Real time application 
Here we can consider a real time application where one user subscribes to a service and whenever there is a new added promo in that service he will be getting the notification. This notification can be anything (Mail/SMS, etc. )
Let us take an example of Netflix application and think that this application data is stored in a S3 bucket and this bucket is integrated to a Lambda function and this Lambda function is having destination as SNS where SNS sends you the notification. 
So, suppose you have registered for netflix to send you mails whenever a video gets uploaded in a particular channel our funciton gets triggered. 
So, the data of Netflix is stored in S3 and when a new object is uploaded our Lambda function gets triggered and this lambda function with destination SNS will send you the mail (only if you subscribe). 

# boto3 
boto3 is the Amazon Web Services (AWS) Software Development Kit (SDK) for Python. It allows Python developers to write software that makes use of services like Amazon S3 and Amazon EC2. Here's a breakdown of key points related to boto3.

# Getting Started 

# Pre requisites 
Minimal knowledge on Linux and shell scripting
Python knowledge 

File structure - 
requirements.txt file is the file to add required python modules
s3-lambda-function.py file used to create a Lambda function using python boto3 module (python module to interact with AWS
s3-notification-triggers.sh file used for shell scripting automation. 

Install AWI CLI (Click on below link for reference for MAC/Windows/Linux)
https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

After installing AWS CLI, you need to configure your access to access the AWS using AWS CLI 
So take the access, secret key using IAM User of AWS and provide to the CLI after giving "AWS Configure". 
Now your all set to make an S3 event triggering using S3/Lambda/SNS/Shell scripting 
Use the command "s3-notification-triggers.sh" 
This will run the file and do the needed modifications in the AWS. 
