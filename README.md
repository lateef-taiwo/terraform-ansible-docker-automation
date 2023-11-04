# Terraform-Ansible-Docker-Automation
This repository is a project for automation of the deployment of docker containers on AWS using terraform and Ansible
### initialize

    terraform init

### Preview terraform actions

    terraform plan

### Apply configuration with variables

    terraform apply -var-file terraform-dev.tfvars

### Destroy a single resource

    terraform destroy -target aws_vpc.myapp-vpc

### Destroy everything from tf files

    terraform destroy

### Show resources and components from current state

    terraform state list

### Show current state of a specific resource/data

    terraform state show aws_vpc.myapp-vpc    

### Set avail_zone as custom tf environment variable - before apply

    export TF_VAR_avail_zone="eu-west-3a"

### Set aws configuration through env variables

    export AWS_ACCESS_KEY_ID="anaccesskey"
    export AWS_SECRET_ACCESS_KEY="asecretkey"
    export AWS_DEFAULT_REGION="us-west-2"                                                                                                                                                                      
