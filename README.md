
![Logo](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)


# Hosting a static website using Amazon S3

You’ll create an Amazon S3 bucket to hold your static website files and an Amazon CloudFront distribution to serve your website globally. Amazon Route 53 will manage your domain name, and AWS Certificate Manager will provide a valid SSL/TLS certificate.


## Services used

 - Amazon S3 
- Amazon CloudFront 
- Amazon Route 53 
- AWS Certificate Manager


## Prerequisites
You’ll need a few things to get started with this project:

- Static website made up of HTML, CSS, JavaScript, etc. files.



## Documentation

Click this [Tutorial](https://docs.aws.amazon.com/AmazonS3/latest/userguide/website-hosting-custom-domain-walkthrough.html) to learn more about how to host a static website using amazon S3 and route 53. 



## S3 Bucket Policy

To deploy this project run

```bash
  {
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::nimgutabucket/*"
    }
  ]
}
```


## 🚀 About Me
Enthusiastic cloud practitioner with a passion for AWS projects. I love learning new things and sharing my knowledge with others. I am always looking for new and innovative ways to use AWS to solve real-world problems.


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://katherineoelsner.com/)
[![linkedin](www.linkedin.com/in/mwanahamisi-gakweli-432a9621a)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/)


## 🛠 Skills
Javascript, HTML, CSS...

