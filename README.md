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
	      Assign elastic ip address.
	  2. Launch Mobaxterm  
	  3. Remote Host:  
		ssh -i "<yourname>-awscli.pem" ec2-user@ec2-3-25-127-73.ap-southeast-2.compute.amazonaws.com

               eg. ssh -i "cheungm-mqtt.pem" ec2-user@ec2-54-79-195-173.ap-southeast-2.compute.amazonaws.com

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

# Perl upgrade using PerlBrew


## Installing perlbrew
Using Perl </usr/bin/perl>
perlbrew is installed: ~/perl5/perlbrew/bin/perlbrew

perlbrew root (~/perl5/perlbrew) is initialized.

Append the following piece of code to the end of your ~/.bash_profile and start a
new shell, perlbrew should be up and fully functional from there:

    source ~/perl5/perlbrew/etc/bashrc

[ec2-user@ip-172-31-44-23 ~]$ perlbrew install perl-5.30.0
Fetching perl 5.30.0 as /home/ec2-user/perl5/perlbrew/dists/perl-5.30.0.tar.gz
Download http://www.cpan.org/authors/id/X/XS/XSAWYERX/perl-5.30.0.tar.gz to /home/ec2-user/perl5/perlbrew/dists/perl-5.30.0.tar.gz
Installing /home/ec2-user/perl5/perlbrew/build/perl-5.30.0/perl-5.30.0 into ~/perl5/perlbrew/perls/perl-5.30.0

## Using perl 5v30
[ec2-user@ip-172-31-44-23 ~]$ perlbrew use perl-5.30.0
[ec2-user@ip-172-31-44-23 ~]$ perl --version

This is perl 5, version 30, subversion 0 (v5.30.0) built for x86_64-linux
(with 1 registered patch, see perl -V for more detail)

/home/ec2-user/perl/Ex_Files_Perl_5_EssT/Exercise Files/Ch01
[ec2-user@ip-172-31-44-23 Ch01]$ perl hello-version.pl
Perl version is v5.30.0


## Java and Maven
https://docs.aws.amazon.com/neptune/latest/userguide/iam-auth-connect-prerq.html

Custom TCP	TCP	8080	0.0.0.0/0	swagger

http://ec2-54-79-195-173.ap-southeast-2.compute.amazonaws.com:8080/swagger-ui/index.html?configUrl=/v3/api-docs/swagger-config

http://ec2-54-79-195-173.ap-southeast-2.compute.amazonaws.com:8080/v3/api-docs

## Public AMIs
SonarQube version -- 	8.5.1.38104-1
https://bitnami.com/stack/sonarqube/cloud/aws/amis

 # Related Articles
 https://mobaxterm.mobatek.net/download.html
 
 https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html
 
https://medium.com/@ahmeeddhon/using-aws-instance-scheduler-to-reduce-amazon-ec2-or-rds-cost-56c9eb374344

https://perlbrew.pl/

https://docs.aws.amazon.com/neptune/latest/userguide/iam-auth-connect-prerq.html
