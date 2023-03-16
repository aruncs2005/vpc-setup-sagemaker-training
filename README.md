# vpc-setup-sagemaker-training

This sample repository shows how to setup up and use VPC with SageMaker Training. There are two branches - 


This repo contains a CFN template to launch the AWS infrastructure necessary. The notebook [training-vpc.ipynb](training-vpc.ipynb) has the necessary cells to launch the CFN stack and runs a training job that accesses your data in s3. Finally, it also has instructions for cleanup to avoid unnecessary costs.

To run the notebook without any errors, make sure the following IAM policies are attached to the notebook's execution role.

- [NetworkAdministrator](https://console.aws.amazon.com/iam/home#/policies/arn:aws:iam::aws:policy/job-function/NetworkAdministrator)
- [AmazonSageMakerFullAccess](https://console.aws.amazon.com/iam/home#/policies/arn:aws:iam::aws:policy/AmazonSageMakerFullAccess)
- [AWSCloudFormationFullAccess](https://console.aws.amazon.com/iam/home#/policies/arn:aws:iam::aws:policy/AWSCloudFormationFullAccess)

