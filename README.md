# Bitbucket pipelines configuration to deploy the code as a static web in S3

Minimum configuration to use bitbucket pipelines in order to deploy the code as a static web in a S3 bucket.  
Using a docker image that contains the AWS CLI: 
[https://github.com/jmmorlesin/docker-maven-ant-awscli](https://github.com/jmmorlesin/docker-maven-ant-awscli)

Bitbucket will need some environment variables in the pipelines section:  

| Name                     | Description                                        |
|--------------------------|----------------------------------------------------|
| AWS_ACCESS_KEY_ID        | AWS Access Key                                     |
| AWS_S3_REGION            | Region of the bucket                               |
| AWS_SECRET_ACCESS_KEY    | AWS Secret Access Key                              |
| S3_BUCKET_NAME           | S3 Bucket configured as host of a Static Website   |

More information about host an static website in Amazon: [Hosting a Static Website on Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/dev/WebsiteHosting.html) 

License
-------

May be freely distributed under the [MIT license](https://github.com/jmmorlesin/bitbucket-pipelines-deploy-web-s3/blob/master/LICENSE).

Copyright (c) 2017 Jose M. Morlesín 
