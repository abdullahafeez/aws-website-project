# aws-website-project

sudo apt-get update
# For Sql-client
sudo apt-get install mysql-client

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