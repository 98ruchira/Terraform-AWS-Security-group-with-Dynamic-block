# Terraform configuration for AWS security group with Dynamic block

## Overview

This Terraform script for bulid AWS security group with open multiple ports using terraform dynamic block feature.

## Prerequisites

## Before running the Terraform script, ensure you have the following:

- AWS CLI configured with appropriate credentials.
- Terraform installed on your machine.

## Configuration

## Update the values in the `variable.tf` file according to your requirements:
...
variable "sg_ports" 
description = "List of ports for ingress rules"
type        = list(number)
default = [ 22, 80, 8200, 8300, 9200 ]
...

## Run the following command to initialize Terraform and download the necessary providers:

terraform init

## Generate the execution plan:

terraform plan

## Ensure that the execution plan looks correct before proceeding.
## Apply the changes:

terraform apply
Confirm the changes when prompted.
