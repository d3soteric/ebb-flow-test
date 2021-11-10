# Ebb and Flow
Shared for educational purposes only.  No warranty/responsibility of any kind implied or otherwise accepted by the original author, user is liable for what they do with any of the resources they may produce from this template, use at your own risk and I hope it is helpful and informative.

the res_infra.json template is a skeleton to get you started with replicating the simulation environment. It includes the VPC, IGW, routetable, route, subnets, security groups and EC2 instances.  Note that one of the EC2 instances includes base64-encoded user data which is executed on startup.  This updates the instance, installs pip and scapy.

RDS, ES, S3, flow logs and the vulnerable test server running on Ubuntu are not included but using the skeleton provided can be built as needed and if desired.

Depending on the tests desired to run, additional security group modifications may be required or desired.

The res_storage.json template is not needed unless you want to mess with setting flow logs to go to s3 buckets created in other accounts (abandoned by me because CloudWatch was simpler for my testing)
