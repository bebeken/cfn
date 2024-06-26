# cfn

## S3
```
aws cloudformation create-stack --stack-name {stack_name} --template-body file://cfn_s3.yml --parameters ParameterKey=BucketName,ParameterValue={backet_name}
aws cloudformation create-change-set --change-set-name {change_set_name} --stack-name {stack_name} --template-body file://cfn_s3.yml --parameters ParameterKey=BucketName,ParameterValue={backet_name}
```

## CertificateManager
```
aws cloudformation create-stack --stack-name {stack_name} --template-body file://cfn_acm.yml --parameters ParameterKey=DomainName,ParameterValue={domain_name} --region us-east-1
aws cloudformation create-change-set --change-set-name {change_set_name} --stack-name {stack_name} --template-body file://cfn_acm.yml --parameters ParameterKey=DomainName,ParameterValue={domain_name} --region us-east-1
```

## CloudFront
```
aws cloudformation create-stack --stack-name {stack_name} --template-body file://cfn_cf.yml --parameters ParameterKey=CertificateArn,ParameterValue={certificate} ParameterKey=AlternativeDomainName,ParameterValue={alternative_domain_name}
aws cloudformation create-change-set --change-set-name {change_set_name} --stack-name {stack_name} --template-body file://cfn_cf.yml --parameters ParameterKey=CertificateArn,ParameterValue={certificate} ParameterKey=AlternativeDomainName,ParameterValue={alternative_domain_name}
```