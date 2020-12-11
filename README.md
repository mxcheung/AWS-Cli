# AWS-Cli
AWS Command Line Interface

# Objectives
- Install AWS CLI Version 2
- Access EC2 instance via Acces Key


C:\Users\Max>aws --version
aws-cli/2.0.24 Python/3.7.7 Windows/10 botocore/2.0.0dev28

 # Step by Step 
https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html


	  1. Create Ec2 instance Key pair    <yourname>-awscli.pem
	  2. Launch Mobaxterm  
	  3. Remote Host:  
		ssh -i "<yourname>-awscli.pem" ec2-user@ec2-3-25-127-73.ap-southeast-2.compute.amazonaws.com

               eg. ssh -i "cheungm-mqtt.pem" ec2-user@ec2-3-25-127-73.ap-southeast-2.compute.amazonaws.com


# Screenshot

[2020-12-12 09:41.58]  /drives/d/max/aws
[Max.DESKTOP-1ULQ7VE] ➤ ls -ltr cheungm-mqtt.pem
-rw-------    1 Max      UsersGrp      1692 Jan 19  2020 cheungm-mqtt.pem

[2020-12-12 09:42.07]  /drives/d/max/aws
[Max.DESKTOP-1ULQ7VE] ➤ ssh -i "cheungm-mqtt.pem" ec2-user@ec2-3-25-127-73.ap-southeast-2.compute.amazonaws.com
X11 forwarding request failed on channel 0
Last login: Fri Dec 11 22:40:35 2020 from 49.3.64.78

       __|  __|_  )
       _|  (     /   Amazon Linux 2 AMI
      ___|\___|___|

https://aws.amazon.com/amazon-linux-2/
7 package(s) needed for security, out of 19 available
Run "sudo yum update" to apply all updates.
[ec2-user@ip-172-31-44-23 ~]$


 # Related Articles
 https://mobaxterm.mobatek.net/download.html
 
 https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html
 
https://medium.com/@ahmeeddhon/using-aws-instance-scheduler-to-reduce-amazon-ec2-or-rds-cost-56c9eb374344

