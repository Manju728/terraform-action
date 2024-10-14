# terraform-action
Git action for doing terraform plan and apply
# Usage
### Do Plan
```yaml
    - name: Terraform plan
      uses: MRKR-PROJECTS/terraform-action@V1.0
      with:
        role-to-assume: "arn:aws:iam::0123456789012:role/role-name"
        aws-region: "ap-south-1"
        terraform_version: "1.6.6"
        account_setup_directory: "cloud_infrastructure/cloud_setup"
        environment: "deploy"
        tf_vars_file: "tfvars/dev.tfvars"
        action_to_performed: "plan"
```
### Do Apply
```yaml
    - name: Terraform plan
      uses: MRKR-PROJECTS/terraform-action@V1.0
      with:
        role-to-assume: "arn:aws:iam::0123456789012:role/role-name"
        aws-region: "ap-south-1"
        terraform_version: "1.6.6"
        account_setup_directory: "cloud_infrastructure/cloud_setup"
        environment: "deploy"
        tf_vars_file: "tfvars/dev.tfvars"
        action_to_performed: "apply"
```
