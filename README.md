# Overview
Repo containing all self-created, personal CloudFormation Templates.

# Current Templates:
## EC2InstanceStack
Creates an EC2 instance, bootstraps instance to update the Message of the day, uses cfn-signal to confirm bootstrapping has completed & creates + attaches SSM Role

**Uses:** Parameters, EC2, cfn-signal, IAM Role, Instance Profile, Outputs <br />
**Future Updates:** Include cfn-init & cfn-hup.


## LoadBalancerStack
Creates an ALB with Listners, Listner rules, attached WAF, Target Groups & Security Groups

**Uses:** ALB, ALB Listner, ALB Listner Rule, WAF (+ WAF Association), Security Groups, Target Groups <br />
**Pending Additions:** Adding ASG section & ouputs


## VPCStack
Only the outline of this template has been created. Comment lines state what services will be used in this stack.


# Future Templates:
- CI/CD Pipeline Stack (CodePipeline, CodeBuild, CodeDeploy etc)
- Serverless stack (Using AWS SAM)
- Custom Resource stack
- Nested Stack