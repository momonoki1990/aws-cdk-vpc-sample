# Welcome to your CDK TypeScript project

This is a simple CDK project for study, just creating VPC.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

## Created by

```
$ cdk init --language typescript
```

## Useful commands

- `npm run build` compile typescript to js
- `npm run watch` watch for changes and compile
- `npm run test` perform the jest unit tests
- `cdk deploy` deploy this stack to your default AWS account/region
- `cdk diff` compare deployed stack with current state
- `cdk synth` emits the synthesized CloudFormation template

## Getting Started

```
# Environmtn variables
$ vim .env
AWS_ACCOUNT_ID=
AWS_REGION=

# Create S3 buicket and related IAM roles for uploading external files like lambda function, which are used from cloudformation
$ npx cdk bootstrap aws://{aws account id }/{aws region } --profile {aws cli profile label }

# Deploy(create, upload and execute cloudformation)
# $ npx cdk deploy --profile {aws cli profile label }
```

## Reference

- [AWS CDK の開始方法](https://aws.amazon.com/jp/getting-started/guides/setup-cdk/module-three/)
  ※This tutorial uses aws cdk v1, so the following v2 document was used as references for creating vpc stack.

- [class Vpc (construct)](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ec2.Vpc.html)
