# Deploying a Flask Web Application on AWS with Terraform
This project automates the deployment of a Flask web application on AWS using Terraform. It sets up the necessary infrastructure components such as VPC, subnet, security groups, and EC2 instance to host the Flask application. The deployment process is streamlined and repeatable, thanks to infrastructure as code principles.

Features
Infrastructure Automation: Automates the setup of AWS infrastructure using Terraform scripts.
Security: Implements secure SSH access and controls inbound/outbound traffic with security groups.
Deployment Process: Deploys the Flask application onto the EC2 instance using Terraform provisioners.
Flask Application: Includes a simple Flask application that responds with "Hello, Linkedin fam!" on the root URL.
Prerequisites
Before getting started, ensure you have the following prerequisites installed:

Terraform
AWS account with appropriate permissions
SSH key pair for accessing EC2 instances
Usage
Clone the Repository: Clone this repository to your local machine.

git clone https://github.com/yourusername/flask-aws-terraform.git
Navigate to the Project Directory: Change into the project directory.

cd flask-aws-terraform
Update Terraform Variables: Open main.tf file and update the following variables:

aws_access_key and aws_secret_key: AWS access key and secret key.
aws_region: AWS region where you want to deploy the resources.
public_key_path: Path to your public key file.
private_key_path: Path to your private key file.
Initialize Terraform: Initialize Terraform in the project directory.

terraform init

Plan Terraform Deployment: Generate an execution plan.

terraform plan

Apply Terraform Changes: Apply the Terraform configuration to create the infrastructure.

bash

terraform apply

Access the Flask Application: Once the deployment is complete, access the Flask application by navigating to the public IP address of the EC2 instance in your web browser.

Clean Up Resources: After testing, you can clean up the resources to avoid incurring charges.

terraform destroy

Contributing
Contributions are welcome! If you encounter any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.





