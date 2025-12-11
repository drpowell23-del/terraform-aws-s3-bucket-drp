# AWS S3 Bucket Module

A simple Terraform module for creating an S3 bucket.

## Usage

\`\`\`hcl
module "s3_bucket" {
  source  = "app.terraform.io/policy-as-code-training/terraform-aws-s3-bucket-drp/aws"
  version = "1.2.0"
  
  bucket_name = "terraform-aws-s3-bucket-drp"
}
\`\`\`

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|----------|
| bucket_name | Name of the S3 bucket | string | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| bucket_id | The name of the bucket |
| bucket_arn | The ARN of the bucket |