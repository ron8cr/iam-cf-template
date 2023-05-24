# iam-cf-template
## a Cloud-formation template to create an IAM User on AWS

![Screen Shot 2023-05-24 at 10 42 29 PM](https://github.com/ron8cr/iam-cf-template/assets/124076577/9f86899e-1cdb-4f88-a4bf-065bd3f9c329)

This template will create the following resources:

- **ContractorsGroup**: An IAM group named **"Contractors"**
- **DemoUser**: An IAM user named **"DemoUser"**
- **DemoUserGroupMembership**: Adds the **DemoUser** to the **ContractorsGroup**.
- **ContractorsPolicy**: A policy attached to the **ContractorsGroup** that allows access to EC2, S3, and EKS resources.
- Note that the policy in this template provides full access (ec2:*, s3:*, and eks:*) to all resources (Resource: "*") within EC2, S3, and EKS. You may want to refine the policy further based on your specific requirements.
