# Teem Multi Tier VPC CloudFormation Template

This CloudFormation template creates a multi-tier VPC with public and private subnets, an Internet-facing Application Load Balancer, and an Auto Scaling Group.

## Getting Started

To use this template, you will need an AWS account and basic knowledge of AWS CloudFormation and AWS VPC.

### Prerequisites

- AWS account
- AWS CLI or AWS Console
- Basic knowledge of AWS CloudFormation and AWS VPC

### Installation

To create the stack using the AWS CLI, follow these steps:

1. Clone the repository or download the template file.
2. Open your terminal and navigate to the folder containing the template file.
3. Run the following command to create the stack:

aws cloudformation create-stack --stack-name <stack-name> --template-body file://<template-file-name> --parameters ParameterKey=KeyName,ParameterValue=<keypair-name> --capabilities CAPABILITY_NAMED_IAM
    

Replace `<stack-name>` with the name you want to give the CloudFormation stack, `<template-file-name>` with the name of the template file, and `<keypair-name>` with the name of an existing EC2 key pair that you want to use to enable SSH access to instances launched in the VPC.

Alternatively, you can create the stack using the AWS Console. Follow these steps:

1. Sign in to the AWS Management Console.
2. Open the CloudFormation console at https://console.aws.amazon.com/cloudformation/
3. Choose "Create Stack".
4. Select "Upload a template to Amazon S3" and upload the template file.
5. Enter a stack name and parameters as required.
6. Click "Next" and complete the remaining steps as required.

### Usage

After creating the CloudFormation stack, you can log in to the AWS Console to view and manage the resources created by the stack.

#### Outputs

The stack creates the following outputs:

- `VpcId`: The ID of the VPC.
- `PublicSubnetA`: The ID of the public subnet A.
- `PublicSubnetB`: The ID of the public subnet B.
- `PrivateSubnetA`: The ID of the private subnet A.
- `PrivateSubnetB`: The ID of the private subnet B.
- `LoadBalancerDNSName`: The DNS name of the application load balancer.

## Contributing

If you find any issues with this CloudFormation template or have suggestions for improvements, please open an issue or a pull request.

## License

This CloudFormation template is licensed under the MIT License.

## Acknowledgments

This CloudFormation template was created with reference to the AWS documentation and sample templates.
