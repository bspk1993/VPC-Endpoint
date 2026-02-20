# VPC-Endpoint

--> create as usually all the vpc components and create the EC2 instances as usually in public subnet and private subnet

--> If we have a requirement to connect with any resource like S3,RDS,DynamoDB ,etc

--> we need to create a VPC endpoint in same VPC and same subnet which the EC2 in private subnet

-->On creation it will ask the VPC configurations as usual and follow the steps

-->Connect to the EC2 private subnet and give command 
    aws s3 ls --endpoint -url **DNSID** enter

--> we can see the S3 buckets

--> If we give any IAM policy to access any S3 bucket and attach to EC2 instance .So we can connect to S3 partition.
