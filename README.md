# CloudFormation scripts for secure S3 deployment
CloudFormation templates for secure deployment of S3 buckets in AWS

## Description

This reusable solution generates a private and encrypted AWS S3 Bucket leveraging AWS KMS while also enabling Amazon Macie to identify and alert on any sensitive data held in S3 buckets within the account.

### kmsBucketWithMacie.yaml
This AWS CloudFormation template creates an AWS KMS encryption key for S3, an encrypted S3 bucket leveraging the KMS key, and enables Amazon Macie to scan and alert on sensitive data held in S3 buckets of the account.

### kmsBucket.yaml
This AWS CloudFormation template creates an encrypted S3 bucket leveraging an existing KMS key that must be entered as a parameter using the KMS key's ARN when deploying the bucket.

### macie.yaml
This AWS CloudFormation template enables Amazon Macie within the deployed account to scan and alert on sensitive data held within S3 buckets.

## Pricing

[S3 pricing](https://aws.amazon.com/s3/pricing/?p=pm&c=s3&z=4)

[KMS pricing](https://aws.amazon.com/kms/pricing/)

[Macie pricing](https://aws.amazon.com/macie/pricing/)
