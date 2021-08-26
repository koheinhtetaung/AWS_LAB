# This is Cross-Stack-References-Part-1-LAB

- create infra stack
- [infra-stack.yaml] (./cloud_formation/cross-stack-references-part-1/infra-stack.yaml)
```bash
 aws cloudformation create-stack --stack-name infra-stack --template-body file://infra-stack.yaml
```

- update infra stack
 ```bash
  aws cloudformation update-stack --stack-name infra-stack --template-body file://infra-stack.yaml
 ```

- create security stack with parameter
```bash
aws cloudformation create-stack --stack-name security-stack --template-body file://security-stack.yaml --parameter ParameterKey=infraStackName,ParameterValue=infra-stack

```

- delete stack 
```bash
aws cloudformation delete-stack --stack-name security-stack
```
