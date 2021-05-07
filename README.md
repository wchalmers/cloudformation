# Overview
Repo containing all self-created, personal CloudFormation Templates.

# Current Templates:
## EC2InstanceTemplate
Creates an EC2 instance, bootstraps instance to update the Message of the day, uses cfn-signal to confirm bootstrapping has completed & creates + attaches SSM Role

**Uses:** Parameters, EC2, cfn-signal, IAM Role, Instance Profile, Outputs <br />
**Future Updates:** Include cfn-init & cfn-hup.


## LoadBalancerTemplate
Creates an ALB with Listners, Listner rules, attached WAF, Target Groups & Security Groups

**Uses:** ALB, ALB Listner, ALB Listner Rule, WAF (+ WAF Association), Security Groups, Target Groups <br />
**Pending Additions:** Ouputs section

## ASG Template
**Still WIP** Once complete, it will create an ASG, Launch Templates, Security Groups & IAM Roles (and Instance Profiles) & CloudWatch/SNS Alarms.


## VPCTemplate
Only the outline of this template has been created. Comment lines state what services will be used in this stack.


# Future Templates:
- CI/CD Pipeline Template (CodePipeline, CodeBuild, CodeDeploy etc)
- Serverless Template (Using AWS SAM)
- Custom Resource Template
- Nested Stack Template