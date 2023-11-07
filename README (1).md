
![Logo](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)


# Use CloudFormation to Launch an Amazon EC2 Web Server

CloudFormation allows you to deploy resources at scale, more consistently and efficiently, using Infrastructure-as-Code (IaC).


## Services used

 - Amazon CloudFormation
- Amazon EC2
- Amazon VPC (and subcomponents) 


## Prerequisites
You’ll need a few things to get started with this project:

- PuTTY or SSH client



## Documentation

Click this [Tutorial](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/working-with-templates-cfn-designer-walkthrough-createbasicwebserver.html//) to learn more about how to launch an Amazon Ec2 web server using cloudformation.



## Screenshots

- Launching stack.(https://nimgutabucket.s3.eu-north-1.amazonaws.com/Launching+Stack.jpeg)
- Ec2 instance(App Server) is launched automatically as stated in the below template.(https://nimgutabucket.s3.eu-north-1.amazonaws.com/Ec2+Instance+is+launched+automatically+using+the+below+template.jpeg)
- App Server(https://nimgutabucket.s3.eu-north-1.amazonaws.com/App+server.jpeg)
- Ec2 instance is linked to the same VPC as stated in the template above. (https://nimgutabucket.s3.eu-north-1.amazonaws.com/Ec2+is+linked+to+the+same+vpc+as+stated+in+the+template+above.jpeg)
- VPC(Lab VPC) is launched automatically as stated in the cloud formation template below.(https://nimgutabucket.s3.eu-north-1.amazonaws.com/VPC+is+launched+automatically+as+stated+in+the+cloud+formation+template+below.jpeg)
- Lab VPC(https://nimgutabucket.s3.eu-north-1.amazonaws.com/Lab+VPC.jpeg)


## CloudFormation template

To deploy this project run

```bash
  AWSTemplateFormatVersion: 2010-09-09
Description: Lab template

# Lab VPC with public subnet and Internet Gateway

Parameters:

  LabVpcCidr:
    Type: String
    Default: 10.0.0.0/20

  PublicSubnetCidr:
    Type: String
    Default: 10.0.0.0/24

  AmazonLinuxAMIID:
    Type: AWS::SSM::Parameter::Value<AWS::EC2::Image::Id>
    Default: /aws/service/ami-amazon-linux-latest/amzn2-ami-hvm-x86_64-gp2

Resources:

###########
# VPC with Internet Gateway
###########

  LabVPC:
    Type: AWS::EC2::VPC
    Properties:
      CidrBlock: !Ref LabVpcCidr

```


## Authors

- [@Gakwelimwanahamisi](https://www.github.com/gakwelimwanahamisi)


## 🚀 About Me
Enthusiastic cloud practitioner with a passion for AWS projects. I love learning new things and sharing my knowledge with others. I am always looking for new and innovative ways to use AWS to solve real-world problems


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://katherineoelsner.com/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/)


## 🛠 Skills
Javascript, HTML, CSS...

