# cloudformationstack-architecture
This cloudformation stack provisions the following AWS resources:
- A two-tier VPC with one public subnet and one private subnet
- An Internet Gateway in the VPC
- An ELB in the public subnet
- A Network Address Translation EC2 instance in the public subnet
- An EC2 auto-scaling group in the private subnet
- A DynamoDB table
- IAM role to control access to the DynamoDB table
- SecurityGroups for the ELB, auto-scaling group, and NAT instance
The requirement that deployments should be easily repeatable means deployment of the AWS resources should be automated.
