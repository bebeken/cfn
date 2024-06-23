# cfn

## S3
```
aws cloudformation create-stack --stack-name {stack_name} --template-body file://cfn_s3.yml --parameters ParameterKey=BucketName,ParameterValue={backet_name}
```

## CertificateManager
```
aws cloudformation create-stack --stack-name {stack_name} --template-body file://cfn_acm.yml --parameters ParameterKey=DomainName,ParameterValue={domain_name}  --region us-east-1
```