### Deploy a high-availability web app using CloudFormation
This folder provides the solution code for the "ND9991 - C2- Infrastructure as Code - Deploy a high-availability web app using CloudFormation" project. This folder contains the following files:

#### network.yml
CloudFormation code for building the network part of the cloud infrastructure, as required for the project. 

#### network-parameters.json
JSON file with parameters for the network.yml CloudFormation script

#### servers.yml
CloudFormation code for building the servers part of the cloud infrastructure, as required for the project. UdacityS3ReadOnlyEC2 role is added to be able to read from the s3 bucket in future.

The last line in UserData script was changed a bit, since the provided one didn't work:
```bash
sudo bash -c "echo Udacity Demo Web Server Up and Running! > index.html"
```

#### server-parameters.json
JSON file with parameters for the server.yml CloudFormation script
