# aws-website-project

#List of AWS services used
S3, RDS(mysql), EC2, Route53

#Create S3 Bucket
Update the name in config.py

#Create a new RDS(mysql) instance
Update the name in config.py

sudo apt-get update
# For mysql-client
sudo apt-get install mysql-client

#Database Connection & Creation
mysql -h 'url of database' -u 'username' -p password
show databases; 
create database employee;
use employee;
create table employee(empid varchar(20),fname varchar(20),lname varchar(20),pri_skill varchar(20),location varchar(20));


# For python and related frameworks

sudo apt-get install python3

#Either use these commands or the one starting from pip3
sudo apt-get install python3-flask
sudo apt-get install python3-pymysql
sudo apt-get install python3-boto3

# if you want to install it through pip then,
#sudo apt-get install python3-pip
#pip3 install pymysql boto3
#pip3 install flask

#You need to update the IP address of the website hosted in or just type in the domain name, which is essentially the ec2 instance in our scenario
templates/AddEmpOutput.html
templates/GetEmp.html
templates/GetEmpOutput.html

# for running application
sudo python3 Empapp.py