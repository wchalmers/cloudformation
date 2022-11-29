# Overview
Repo containing all self-created, personal CloudFormation Templates.

# Current Templates:
## EC2InstanceTemplate
Creates an EC2 instance, bootstraps instance to update the Message of the day, uses cfn-signal to confirm bootstrapping has completed & creates + attaches SSM Role

**Uses:** Parameters, cfn-signal, IAM Role, EC2, Instance Profile, Outputs <br />
**Future Updates:** Include cfn-init & cfn-hup.


## LoadBalancerTemplate
Creates an ALB with Listners, Listner rules, Attached WAF, Target Groups & Security Groups

**Uses:** ALB, ALB Listner, ALB Listner Rule, WAF (+ WAF Association), Security Groups, Target Groups <br />

## ASG Template
Creates an ASG, Launch Templates, Security Group, Placement Group & IAM Roles (and Instance Profiles) & SNS Topic (with ASG alarms).

**Uses:** Conditions, !If/!Not/!Equals/!Sub Statements, CloudWatch Alarms & All services listed above


## VPCTemplate
Template that creates a full VPC With 4 Subnets, IPv4, IPv6 aswell as other attachments such as a NatGateway, Route53 Records, Flowlogs & Endpoints.

## Example File
This contains examples of some YAML formatting and features that can be used when writing YAML templates (note, some of these may not work within CloudFormation)

## Parameters Template
This contains examples of parameter formatting through the metadata section, aswell as the different types of parameters & their settings.


# Future Templates:
- CI/CD Pipeline Template (CodePipeline, CodeBuild, CodeDeploy etc) - This will probably be a simple pipeline that deploys some cfn templates.
- Serverless Template (Using AWS SAM)
- Custom Resource Template
- Nested Stack Template

# Useful Links
- [Pseudo Parameters](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/pseudo-parameter-reference.html)
- [Parameter Types](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/parameters-section-structure.html)
- [Ref/GetAtt Cheatsheet](https://theburningmonk.com/cloudformation-ref-and-getatt-cheatsheet/)
- [CloudFormation Drift Detection Supported Resources](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/resource-import-supported-resources.html)
- [CloudFormation Best Practices](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/best-practices.html)
