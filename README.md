# README #

Terraform scripts to create an AWS VPC.

The TF plan will create the following resources:

* x1 vpc
* x1 Public route table
* x1 Internet gateway
* x2 Public subnets
* x2 Private subnets

The plan also contains an init.sh script. This script enables remote state to AWS S3:

### Prerequisites ###

* AWS account - https://aws.amazon.com
* AWS IAM user account with AWS access/secret keys and permission to create specified resources
* Terraform installed - https://www.terraform.io
* Git account and git installed - https://github.com
* The ability to run .sh (shell) scripts if using Windows

### How do I get set up? ###

* Clone the repo
* Create terraform.tfvars
* Create an S3 bucket
* Update the init.sh BUCKET and REGION vars
* Run the init.sh file
* Run terraform plan (to plan the deployment)
* Run terraform apply (to apply the plan and deploy all resources)
* Run terraform destroy (to destroy all deployed resources)

### Who do I talk to? ###

* Rich Bos
