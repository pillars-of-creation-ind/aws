# AWS Cloud Formation

- AWS Cloud Formation is a service that helps you model and setup your AWS resources
  so that you can spend less time managing those resources and more focusing on your applications
  that run in aws
- You can create a template (.JSON / .yml) file that describes all the aws resources. Cloudformation
  takes care of provisioning and configuring those resources.
- Cloudformation uses these templates as blueprints for build aws resources.
- Useful in
  1. Infrastructure management
  2. Quickly replicate your infrastructure
  3. Easily control and track changes to your infrastructure

Example:
In a template (with name), you can describe an Amazon EC2 instance, such as

- the instance type
- the AMI ID
- block device mappings
- amazon key pair name

Cloud formation provisions an instance with an `ami-0ff8a91507f77f867` AMI ID,
t2.micro instance type, test key pair name, and an amazon EBS volume
