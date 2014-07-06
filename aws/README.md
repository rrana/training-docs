# Amazon Web Services (AWS)

Amazon Web Services (AWS) provides computing resources and services that you can use to build applications within minutes at pay-as-you-go pricing. For example, you can rent a server on AWS that you can connect to, configure, secure, and run just as you would a physical server. The difference is the virtual server runs on top of a planet-scale network managed by AWS.

You pay for your virtual server only while it runs, with no up-front purchase costs or ongoing maintenance costs. Backed by the AWS network, your virtual server can do things no physical server can, such as automatically scaling into multiple servers when demand for your application increases.

Using AWS to build your Internet application is like purchasing electricity from a power company instead of running your own generator, and it provides many of the same benefits: capacity exactly matches your need, you pay only for what you use, economies of scale result in lower costs, and the service is provided by a vendor experienced in running large-scale networks.

You should go through the following document for more introductory information about AWS:
[Overview of Amazon Web Services](https://d36cz9buwru1tt.cloudfront.net/AWS_Overview.pdf)

Also check out the AWS products page: [AWS Products] (http://aws.amazon.com/products/)

## Table of contents

* [Obtain your NewsCred AWS credential] (#obtain-your-newscred-aws-credential)
* [AWS Console login] (#aws-console-login)
* [Setup Multi Factor Authentication (MFA) and update your credentials] (#setup-multi-factor-authentication-and-update-your-credentials)
* [AWS products used in NewsCred] (#aws-products-used-in-newscred)
    * EC2 
	* EBS 
	* ELB 
	* S3 
	* RDS 
	* ElastiCache 
	* Cloudfront
	* Route 53
	* Cloudwatch
* [AWS API and CLI tools] (#aws-api-and-cli-tools)
* [Hands on training resources] (#hands-on-training-resources)
* [AWS Resources] (#aws-resources)
    * AWS Documentation
    * Articles and tutorials
    *   

## Obtain your NewsCred AWS credential

Contact someone in DevOps team for your AWS access credentials (user ID, password, access key ID and secret access key). 
You can contact over email (devops@newscred.com) or in hipchat room (DevOps). 
You need user ID and password for AWS console login and access key ID with secret access key for programmatic access to AWS resources.

Please keep your credentials secure and rotate them on regular basis.

## AWS Console login

The AWS Management Console is a single destination to manage all AWS resources, from EC2 instances to S3 objects. You can use the Console to perform any number of tasks, from deploying new applications to monitoring the health of your application.

NewsCred's AWS Console login alias url: https://newscred.signin.aws.amazon.com/console

Login with the provided user ID and password. 

After initial login please go to https://console.aws.amazon.com/iam/home?region=us-east-1#users and update your credentials.

1. Filter with your user name and right click over your 'User Name'. 
2. Choose 'Manage Password'  
3. Choose 'Replace existing password with new custom password'.
4. Change your password with a secure one.

## Setup Multi Factor Authentication and update your credentials

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

## AWS products used in NewsCred

### EC2

Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) cloud. Using Amazon EC2 eliminates your need to invest in hardware up front, so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. Amazon EC2 enables you to scale up or down to handle changes in requirements or spikes in popularity, reducing your need to forecast traffic.

    * [Getting Started with Amazon EC2 Linux Instances] (#http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html)
    * [Launch an Amazon EC2 Instance] (#http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-launch-instance_linux.html)
    * [Connect to Your Instance] (#http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-connect-to-instance-linux.html)
    * [Add a Volume to Your Instance] (#http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-add-volume-to-instance.html)
    * [Clean Up Your Instance and Volume] (#http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-clean-up-your-instance.html)

(Please note that we have our own process to launch a new instance, EBS volume management and instance/volume. We will discuss them in relavant section shortly)

## Hands on training resources

Before you start using our actual AWS console we suggest you try the simulator console for a while and practice few basics here.

Go to this simulator console lab link and login with the following credentials: 
https://run.qwiklab.com/
Login ID: rana@newscred.com
Login password: qwe90qwe

Launching EC2 Instances: [Lab] (#https://run.qwiklab.com/focuses/preview/1024)
Elastic block store: [Lab] (#https://run.qwiklab.com/focuses/preview/1045)
Using Amazon RDS: [Lab] (#https://run.qwiklab.com/focuses/preview/1034)


## AWS Resources

    * [AWS Documentation] (#https://aws.amazon.com/documentation/?nc1=h_d_dm)
    * [Articles and tutorials] (#http://aws.amazon.com/articles/?nc1=h_d_ta)
