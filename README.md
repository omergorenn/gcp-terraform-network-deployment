# Google Cloud Network Infrastructure Deployment with Terraform

## Overview

This repository provides Terraform configurations to automate the deployment of a Google Cloud network infrastructure. The setup includes the creation of a custom network, firewall rules, and virtual machine instances in different regions.

## Prerequisites

Ensure you have the following prerequisites:

- [Google Cloud Platform (GCP) account](https://cloud.google.com/)
- [Terraform](https://www.terraform.io/) installed

## Getting Started

1. Clone this repository:

    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2. Verify your Terraform installation:

    ```bash
    terraform --version
    ```

3. Initialize Terraform:

    ```bash
    terraform init
    ```

4. Review and customize configurations:

    - Adjust variable values in `mynetwork.tf` and `instance/variables.tf` as needed.

5. Format the Terraform files:

    ```bash
    terraform fmt
    ```

6. Initialize Terraform:

    ```bash
    terraform init
    ```

## Deployment

1. Create an execution plan:

    ```bash
    terraform plan
    ```

2. Apply the changes:

    ```bash
    terraform apply
    ```

    Type `yes` when prompted.

## Verification

1. Verify the resources in the Google Cloud Console:

    - VPC network and subnetworks
    - Firewall rules
    - VM instances

2. Test connectivity between VM instances.

## Clean-Up

To avoid unnecessary costs, destroy the created resources:

```bash
terraform destroy
```

Type `yes` when prompted.

## Important Notes

- Ensure correct variable values in `mynetwork.tf` and `instance/variables.tf`.
- Review and customize firewall rules in `mynetwork.tf`.

