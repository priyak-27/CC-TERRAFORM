## Congruence Closure Algorithm implementation
This project automates the provisioning of infrastructure to test the Congruence Closure Algorithm using Terraform. It sets up necessary resources, including VPC, Subnet, Route table, Internet Gateway, EC2 instances, and installs required dependencies such as Python libraries for visualization and graph generation, ensuring a streamlined environment for running and testing the algorithm.

## Project Requirements
The project requires an automated infrastructure setup whenever they need to test changes made to their Flask application. They need a solution that enables them to:

1. Provision the necessary AWS resources (VPC, Subnet, Route Table, EC2) without manual intervention.
2. Automatically deploy the Flask application on an EC2 instance each time they need to test it and see only the final result on the browser, not the visualisation.
3. Eliminate the need to manually create and configure the infrastructure every time they want to run or test the app.py file.
4. Utilize Terraform to create, configure, and destroy the required infrastructure for testing.


## Usage: 
1. Open the web application in a browser.
2. Enter a formula (such as constraints in the form of equalities or inequalities) into the input field.
3. Submit the form to initiate the algorithm.
4. wait for the program to complete execution (NOTE: you won't see visualisation) and show the result "SAT" or "UNSAT"

## Execution
1. clone the repo
2. go to the folder where main.tf file is located
3. run terraform plan and then apply
4. go to local browser and browse http://public_ip_of_ec2_instance
5. once testing is done , run terraform destroy
