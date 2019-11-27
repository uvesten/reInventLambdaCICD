# Lambda CICD 

git clone https://git-codecommit.us-east-1.amazonaws.com/v1/repos/reInventLambdaCICD

```bash
sam package  --output-template-file packaged.yaml  --s3-bucket vashi-lambda-code
```


```bash
sam deploy --template-file packaged.yaml --stack-name LambdaCICD --capabilities CAPABILITY_IAM
```


Create CodeBuild and code pipeline from console

Start doing controlled deployments by adding the Lambda alias and preTrafficHook


