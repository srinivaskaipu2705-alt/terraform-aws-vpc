# terraform AWS VPC

this module creates the following resources. 
* VPC
* IGW
* 2 public subnets in us-east1a and us-east-1b AZ
* 2 private subnets in us-east1a and us-east-1b AZ
* 2 database subnets in us-east1a and us-east-1b AZ
* public route table
* private route table
* database route table
* EIP for NAT
* NAT Gateway in public subnet 1a az
* IGW route is added to public route table
* NAT Gateway route to private and database route tables
* Route table association with subnets
* VPC to default VPC peering
* public route table to default VPC route
* Default VPC main route table to created VPC route


### inputs


* vpc_cidr  -(required). user must supply the cidr for vpc
* projrct_name -(required). user must supply the project nae.