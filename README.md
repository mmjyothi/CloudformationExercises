# CloudformationExercises



exercise 2

Is for creating the S3 bucket with public read access


[ec2-user@ip-172-31-43-204 CloudformationExercises]$ aws cloudformation delete-stack --stack-name myteststack

[ec2-user@ip-172-31-43-204 CloudformationExercises]$ aws cloudformation create-stack --stack-name myteststack --template-body file:////home//ec2-user//CloudformationExercises//exercise2.template


exercise 3

This template is for create a ec2 Instance with a new securitygroup and existing security group attached to it. You need to have a keypair in your account for it to work.


[ec2-user@ip-172-31-43-204 CloudformationExercises]$ aws cloudformation create-stack --stack-name myteststack --template-body file:////home//ec2-user//CloudformationExercises//exercise3.template  --parameters ParameterKey=KeyName,ParameterValue=EC2Key

[ec2-user@ip-172-31-43-204 CloudformationExercises]$ aws cloudformation delete-stack --stack-name myteststack

Elastic Load Balancing template

[ec2-user@ip-172-31-43-204 CloudformationExercises]$ aws cloudformation create-stack --stack-name myteststack --template-body file:////home//ec2-user//CloudformationExercises//ElasticLoadBalacing.template --parameters ParameterKey=KeyName,ParameterValue=EC2Key

[ec2-user@ip-172-31-43-204 CloudformationExercises]$ aws cloudformation delete-stack --stack-name myteststack



