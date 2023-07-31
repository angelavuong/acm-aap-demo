# Advanced Cluster Management + Ansible Automation Platform Demo

## Prerequisites

Before using these playbooks, you need to have the following:

- An AWS account
- [Ansible Automation Platform](https://developers.redhat.com/products/ansible/download) is installed on your local machine
- Create an SSH key pair in AWS account for your EC2 instance

## Using the playbook 
When using the create_ec2instance.yml playbook, be sure to specify the variables:
```
---
ec2_instance_name: example
region: us-east-1
instance_type: t3.micro
ami: ami-06640050dc3f556bb
key_name: ansible-demo
vpc_name: ansible-vpc
cidr_block: "10.10.0.0/16"
cidr: "10.10.0.0/24"
controller_host: <controller-host.com>
controller_oauthtoken: <token-here>
```
## PostgreSQL Install 
Resource: https://stribny.name/blog/ansible-postgresql/

## MongoDB repository

Install instructions came from [MongoDB documentation](https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-red-hat/)
