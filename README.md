## amazon-eks-cluster-logging-remediation

## Content
- CloudFormation Template

## Why?
 The goal would be to enable a user to be able to launch a Cloudformation template to build the resources. The Cloudformation template has a set CloudWatch Event Rule, and Lambda Function.

 Amazon Elastic Kubernetes Service (EKS) provides control plane logs for each cluster [Reference](https://docs.aws.amazon.com/eks/latest/userguide/control-plane-logs.html)

## Utilities
The Cloudformation template has a set CloudWatch Event Rule, and Lambda Function describes clusters and runs the remediation on each log group for each EKS control plane log types.

The CloudWatch Event Rule has a ScheduleExpression polling at 20 minutes intervals. This is intentional for users with larger cluster requirements.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

