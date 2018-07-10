# Amazon SageMaker Workshops

Amazon SageMaker is a fully managed service that enables developers and data scientists to quickly and easily build, train, and deploy machine learning models at any scale. This repository contains a collection of workshops and other hands on content that will guide you through using the many features of SageMaker.  

![Overview](./images/overview.png)

You'll start by creating a SageMaker notebook instance with the requisite permissions. Depending on the workshop, you will then interact with SageMaker via sample Jupyter notebooks, the AWS CLI, the SageMaker console, or all three. During a workshop, you'll explore various data sets, create model training jobs using SageMaker's hosted training feature, and create endpoints to serve predictions from your models using SageMaker's hosted endpoint feature.  

**BEFORE attempting any of the workshops, please review the Prerequisites below and complete any actions that are required.**


# Prerequisites

## AWS Account

In order to complete this workshop you'll need an AWS Account, and an AWS IAM user in that account with at least full permissions to the following AWS services: 

- AWS IAM
- Amazon S3
- Amazon SageMaker

**Use Your Own Account**: The code and instructions in this workshop assume only one student is using a given AWS account at a time. If you try sharing an account with another student, you'll run into naming conflicts for certain resources. You can work around these by appending a unique suffix to the resources that fail to create due to conflicts, but the instructions do not provide details on the changes required to make this work. Use a personal account or create a new AWS account for this workshop rather than using an organization’s account to ensure you have full access to the necessary services and to ensure you do not leave behind any resources from the workshop.

**Costs**: Some, but NOT all, of the resources you will launch as part of this workshop are eligible for the AWS free tier if your account is less than 12 months old. See the [AWS Free Tier page](https://aws.amazon.com/free/) for more details. An example of a resource that is **not** covered by the free tier is the ml.m4.xlarge notebook instance used in some workshops. To avoid charges for endpoints and other resources you might not need after you've finished a workshop, please refer to the [**Cleanup Guide**](./CleanupGuide). 


## AWS Region

SageMaker is not available in all AWS Regions at this time.  Accordingly, we recommend running this workshop in one of the following supported AWS Regions:  N. Virginia, Oregon, Ohio, or Ireland.

Once you've chosen a region, you should create all of the resources for this workshop there, including a new Amazon S3 bucket and a new SageMaker notebook instance. Make sure you select your region from the dropdown in the upper right corner of the AWS Console before getting started.

![Region selection screenshot](./images/region-selection.png)


## Browser

We recommend you use the latest version of Chrome or Firefox to complete this workshop.

## AWS Command Line Interface

To complete certain workshop modules, you'll need the AWS Command Line Interface (CLI) and a Bash environment. You'll use the AWS CLI to interface with SageMaker and other AWS services. 

For these workshops, you'll use built-in shell terminal on Jupyter notebook in SageMaker notebook instance to execute commands.

# Workshops

- [**Introduction to SageMaker**](Introduction) - This workshop demonstrates the main features of SageMaker via a set of straightforward examples for common use cases.


- [**SageMaker Built-in Algorithms**](Built-in-Algorithms) - The focus of this workshop is on SageMaker's built-in algorithms. These algorithms are ready-to-use, scalable, and provide many other conveniences. The workshop shows how to use SageMaker's built-in algorithms via hosted Jupyter notebooks, the AWS CLI, and the SageMaker console.

# License & Contributing

The contents of this workshop are licensed under the [Apache 2.0 License](./LICENSE). 
If you are interested in contributing to this project, please see the [Contributing Guidelines](./contributing/CONTRIBUTING.md).  In connection with contributing, also review the [Code of Conduct](./contributing/CODE_OF_CONDUCT.md).


