# Amazon Web Services (AWS)

Amazon Web Services (AWS) provides computing resources and services that you can use to build applications within minutes at pay-as-you-go pricing. For example, you can rent a server on AWS that you can connect to, configure, secure, and run just as you would a physical server. The difference is the virtual server runs on top of a planet-scale network managed by AWS.

You pay for your virtual server only while it runs, with no up-front purchase costs or ongoing maintenance costs. Backed by the AWS network, your virtual server can do things no physical server can, such as automatically scaling into multiple servers when demand for your application increases.

Using AWS to build your Internet application is like purchasing electricity from a power company instead of running your own generator, and it provides many of the same benefits: capacity exactly matches your need, you pay only for what you use, economies of scale result in lower costs, and the service is provided by a vendor experienced in running large-scale networks.

You should go through the following document for more introductory information about AWS:
[Overview of Amazon Web Services](https://d36cz9buwru1tt.cloudfront.net/AWS_Overview.pdf)

Also check out the AWS products page: [AWS Products] (http://aws.amazon.com/products/)

### Table of contents
* [Obtain your NewsCred AWS credential] (#obtain-your-newscred-aws-credential)
* [Login to AWS console for the first time] (#login-to-aws-console-for-the-first-time)
* [Setup Multi Factor Authentication (MFA) and update your credentials] (#setup-multi-factor-authentication-and-update-your-credentials)


### Obtain your NewsCred AWS credential

Contact someone in DevOps team for your AWS access credentials (user ID, password, access key ID and secret access key). 
You can contact over email (devops@newscred.com) or in hipchat room (DevOps). 
You need user ID and password for AWS console login and access key ID with secret access key for programmatic access to AWS resources.

Please keep your credentials secure and rotate them on regular basis.

### Login to AWS console for the first time

AWS Console login url: https://newscred.signin.aws.amazon.com/console

Login with the provided user ID and password. 

After initial login please go to https://console.aws.amazon.com/iam/home?region=us-east-1#users and update your credentials.

1. Filter with your user name and right click over your 'User Name'. 
2. Choose 'Manage Password'  
3. Choose 'Replace existing password with new custom password'.
4. Change your password with a secure one.

### Setup Multi Factor Authentication and update your credentials

You have to enable multi factor authentication (MFA):

1. Download Google Authenticator for your phone (or Authenticator if you have a Windows Phone)
2. Go to set up account in your Google Authenticator
3. Go to Scan a barcode
4. Log into AWS
5. Go to IAM menu
6. Go to your username, right click and click manage MFA device
7. Add virtual device
8. Scan barcode that is given with your phone.

You should be good to go.

### 