## Build Layer
```bash
# sam build [the Name in template.yaml Resources: MyLayer] 
sam build MyLayer
---
Building layer 'MyLayer'
Running PythonPipBuilder:ResolveDependencies
Running PythonPipBuilder:CopySource

Build Succeeded

Built Artifacts  : .aws-sam/build
Built Template   : .aws-sam/build/template.yaml

Commands you can use next
=========================
[*] Invoke Function: sam local invoke
[*] Deploy: sam deploy --guided
```

## To deploy
```bash
sam deploy --stack-name [the-stack-name-you-want] --s3-bucket [s3-name-for-sam-to-save-temp-data] --capabilities CAPABILITY_IAM
```