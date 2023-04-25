# Bounty

### AWS

1.  Install the AWS CLI on your machine by running the following command:

    sudo apt-get install awscli
2.  Once the installation is complete, run the following command to configure the AWS CLI:

    aws configure
3. You will be prompted to enter your AWS access key ID and secret access key. You can obtain these credentials from the AWS Identity and Access Management (IAM) console.
4. After you have entered your access key ID and secret access key, you will be prompted to enter the default region name and output format. You can leave these fields blank to use the default settings.
5. Once you have completed the configuration, the AWS CLI will store your access key ID and secret access key in a configuration file located at \~/.aws/credentials.
6. You can now use the aws command followed by the name of the service you wish to interact with, such as aws s3, to perform operations on AWS resources using the credentials you configured.

aws s3 ls s3://bucket-name
