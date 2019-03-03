vpc-check-open-groups
=======
This is an AWS Config Rule written using the Rule Development Kit. It checks the security groups attached to all EC2 instances and flags any instance with an open security group attached to it.


How to deploy this rule:
===================
You must have an AWS account and sufficient permissions to manage the Config service, and to create S3 Buckets, Roles, and Lambda Functions. 

Follow the set-up instructions for the AWS rule development kit:
https://github.com/awslabs/aws-config-rdk.


Once you have rdk set up, you can download this repository and then deploy it directly from the directory you downloaded it to ::

$ rdk deploy vpc-check-open-groups

The rule should then appear on your AWS Config page. 


If you wish to implement the rule manually, you can find instructions here: https://github.com/awslabs/aws-config-rules
