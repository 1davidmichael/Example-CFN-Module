# Example CFN Module

This repo provides an example CloudFormation module. The module creates an S3 bucket with a lifecycle rule to delete objects in it after 30 days.

## Deployment

Once cloned this can be deployed to an account using the `cfn` cli tool

```bash
git clone https://github.com/1davidmichael/Example-CFN-Module.git
cd Example-CFN-Module

cfn submit
```

## Usage

Once deployed this module may be used in additional templates

```yaml
Resources:
  LogBucket:
    Type: DavidMichael::S3::LogBucket::MODULE
```
