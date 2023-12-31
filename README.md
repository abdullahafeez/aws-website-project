# aws-website-project

## **List of AWS services used**
- S3
- RDS(mysql)
- EC2
- Route53
- IAM

### Create S3 Bucket
Update the name in config.py

### Create a new RDS(mysql) instance
Update the name in config.py

`sudo apt-get update`<br />
#### For mysql-client
`sudo apt-get install mysql-client` <br />

#### Database Connection & Creation
`mysql -h 'url of database' -u 'username' -p password` <br />
`show databases;` <br />
`create database employee;` <br />
`use employee;` <br />
`create table employee(empid varchar(20),fname varchar(20),lname varchar(20),pri_skill varchar(20),location varchar(20));` <br />

### Now create an Ec2 instance where we'll host our website
run the following commands

#### For python and related frameworks

`sudo apt-get install python3` <br />

##### Either use these commands or the one starting from pip3
`sudo apt-get install python3-flask` <br />
`sudo apt-get install python3-pymysql` <br />
`sudo apt-get install python3-boto3` <br />

##### if you want to install it through pip then,
`sudo apt-get install python3-pip` <br />
`pip3 install pymysql boto3` <br />
`pip3 install flask` <br />

### IAM Role for ec2 to access s3 bucket
We need to create a new IAM role for our newly created Ec2 service and give permissions for it to access S3 service
Now, attach newly created role to our Ec2 instance

### Route53 route to our domain name
Use any pre-bought domain or create a free domain from freenom.com (Domains registered here are only valid for 3 months only)


##### You need to update the IP address of the website hosted in or just type in the domain name, which is essentially the ec2 instance in our scenario
`templates/AddEmpOutput.html` <br />
`templates/GetEmp.html` <br />
`templates/GetEmpOutput.html` <br />

#### For running application
in our Ec2 Instance <br />
`sudo python3 Empapp.py`<br />
