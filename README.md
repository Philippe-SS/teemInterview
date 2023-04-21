Teem Multi Tier VPC CloudFormation Template

This CloudFormation template creates a multi-tier VPC with public and private subnets, an Internet-facing Application Load Balancer, and an Auto Scaling Group.
Prerequisites

Before using this template, you must have:

    An AWS account
    Basic knowledge of AWS CloudFormation
    Basic knowledge of AWS VPC

Usage

To use this CloudFormation template, follow these steps:

    Sign in to the AWS Management Console.
    Open the CloudFormation console at https://console.aws.amazon.com/cloudformation/
    Choose "Create Stack".
    Select "Upload a template to Amazon S3" and upload the template file.
    Enter a stack name and parameters as required.
    Click "Next" and complete the remaining steps as required.

This template includes the following resources:

    VPC
    Internet Gateway
    Public and Private Subnets
    NAT Gateway
    Security Groups
    Application Load Balancer
    Auto Scaling Group
    VPC Endpoints
    SSL Certificate
    DNS Record

Parameters

This template requires the following parameters:

    KeyName: The name of an existing EC2 key pair to enable SSH access to instances launched in the VPC.

Outputs

This template creates the following outputs:

    VpcId: The ID of the VPC.
    PublicSubnetA: The ID of the public subnet A.
    PublicSubnetB: The ID of the public subnet B.
    PrivateSubnetA: The ID of the private subnet A.
    PrivateSubnetB: The ID of the private subnet B.
    LoadBalancerDNSName: The DNS name of the application load balancer.

Disclaimer

This CloudFormation template is provided as-is and is not intended to be used in a production environment without modification. It is your responsibility to ensure that the template meets your requirements and adheres to AWS best practices.
