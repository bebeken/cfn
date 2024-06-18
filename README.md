# cfn

```
aws cloudformation create-stack --stack-name {stack_name} --template-body file://cfn_s3.yml --parameters ParameterKey=BucketName,ParameterValue={backet_name}
```