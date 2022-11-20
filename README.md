# Cloudformation-stack
Wordpress blogging site

# commands to spin up vpc and jumphost infrastructure

aws cloudformation create-stack --stack-name final --template-body file://master.yml --parameters file://parameters.json --tags Key=Name,Value="cloudapp1"

# step to create webserver and application loadbalancer
you can create from AWS console, Just upload the folder and enter the Jumphost security group ID which was created from the previous stack

# Step to create RDS Instance.
Upload the rds.yml file in cloudformation dashboard and create it.