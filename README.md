1. Create a s3 bucket with name "udagram-project" and upload the ``index.html``

2. Run ``aws cloudformation create-stack --stack-name udagram-network --template-body file://network.yml --parameters file://network-params.json --capabilities CAPABILITY_IAM``

3. Wait for the first stack creation and run ``aws cloudformation create-stack --stack-name udagram-server --template-body file://server.yml --parameters file://server-params.json --capabilities CAPABILITY_IAM``