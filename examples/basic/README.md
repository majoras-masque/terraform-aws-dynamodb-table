# DynamoDB Table example

Configuration in this directory creates AWS DynamoDB table.

## Usage

To run this example you need to execute:

```bash
$ terraform init
$ terraform plan
$ terraform apply
```

Note that this example may create resources which can cost money (AWS Elastic IP, for example). Run `terraform destroy` when you don't need these resources.

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| terraform | >= 0.12.6 |
| aws | >= 2.58 |
| random | >= 2.0 |

## Providers

| Name | Version |
|------|---------|
| random | >= 2.0 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| disabled_dynamodb_table | ../../ |  |
| dynamodb_table | ../../ |  |

## Resources

| Name |
|------|
| [random_pet](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/pet) |

## Inputs

No input.

## Outputs

| Name | Description |
|------|-------------|
| this\_dynamodb\_table\_arn | ARN of the DynamoDB table |
| this\_dynamodb\_table\_id | ID of the DynamoDB table |
| this\_dynamodb\_table\_stream\_arn | The ARN of the Table Stream. Only available when var.stream\_enabled is true |
| this\_dynamodb\_table\_stream\_label | A timestamp, in ISO 8601 format of the Table Stream. Only available when var.stream\_enabled is true |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
