# 4640-w4-lab-start

To create the SSH keypair in the Linux environment we ran the command below
```bash
ssh-keygen -t ed25519 -f ~/.ssh/lab4
```
Next we copied the newly created public key into the cloud-config file and also included the nginx and nmap packages so they automatically install.

To complete the rest of the configuration, you will need:
- Linux environment setup
- Terraform installed
- AWS CLI configured

To run:
- Clone this repository into your Linux environment
- Navigate to project directory
- Create SSH keypair
- Update the cloud-config.yaml file with your existing public key
- Run Terraform commands below to deploy

Commands used for Terraform:
- Initialize Terraform - terraform init
- Format the config files - terraform fmt
- Check config for syntax validation - terraform validate
- Reviewing planned changes - terraform plan
- Apply configuration - terraform apply
- Get output values - terraform output

Once deployed, connect to your instance:
- ssh -i lab4.pub web@<ec2_public_ip>
  - change the ec2_public_ip to your ec2's ip

See lab instructions on D2L for details
