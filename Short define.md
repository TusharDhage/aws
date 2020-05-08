# VPC 
- VPC Stands for `Virtual Private Cloud`.
- In vpc internet configuration is done  like  firewall.
- some vpc may don’t have net.

# Subnet 
- Subnets attach to vpc
- subnet from different zone if internet has problem
- It can be public to private
- It contains route table 
- Security group get under every subnet which contain inbound and outbound
- Security groups different for subnet

# CIDR
- CIDR stands for Classless inter-domain routing 
- Cidr block gives ip adress
- Ip address get must be unique

# Route table
- It contains Net gateway which helps provide actual internet provide and connect with net

# Cloud trail
- Every action saved in cloud trail
- Track user activities
- Similar as cctv

## Cloud watch
* Monitor resource and application
* Cloud trails contains activity like  ec2 create only but cloud watch contains how ec2 used like errors
* We have search feature in insights to  run query on it 
* log store
* log search(query)
* can make Dashboards

# Status check
* It check your instance and network working
* If the internet of aws get failure then it is informed in instance status check 
* We can create alarm for it  

# User data
- For linux user data will  be set of linux or shell script
- For windows we have to pass windows cmd 
- User data is used for automation means commands will pass when instance created it will run commands too.
- In user data commands execute as root user 
- We can pass commands or shell scripts too
- We cant use commands which needs feedback but we can pass it directly with feedback eg yum update -y

# Lambda
- exports.handler = async (event, context) =>{ }  this lambda main function which it used to execute 
- Uses
  - event driven automation
  - lambda as api 

