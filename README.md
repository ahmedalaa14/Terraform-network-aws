## Terraform Network AWS
- This project uses Terraform to provision a robust network infrastructure on AWS. 


## Architecture

The architecture of this project includes:

- A VPC with a default Network ACL
- Subnets:
  - Two public subnets
  - Two private subnets
- Route Table
- Gateways:
  - Internet Gateway
  - NAT Gateway

## Prerequisites
- Before you begin, ensure you have the following installed:

- Terraform
- AWS CLI
- Configured AWS credentials 
```bash
(~/.aws/credentials)
```

## Installation

To install this project, you need to:

1. Clone the repository: 
```bash 
 git clone https://github.com/ahmedalaa14/Terraform-network-aws 
 ```
2. Navigate to the project directory: 
```bash 
cd Terraform-network-aws 
```
3. Initialize Terraform: 
```bash 
terraform init 
```

## Usage

To use this project, you need to:

1. Plan the Terraform changes: 
```bash
terraform plan -var-file=dev.tfvars
```
2. Apply the Terraform changes: 
```bash
terraform apply -var-file=dev.tfvars 
```   

3. Clean up
To destroy the resources created by this project:
```bash
terraform destroy -var-file=dev.tfvars
```



