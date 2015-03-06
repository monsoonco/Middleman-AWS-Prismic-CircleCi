[![alt text](/README_Images/monsoon_.png)](http://www.monsoonco.com/)

Middleman AWS Prismic CircleCi
=================
Welcome to our Middleman-AWS-Prismic-CircleCi open source project!
We've used this lovely setup for creating these live projects at Monsoon: [LunaSleep](http://lunasleep.com/), [Swypcard](https://www.swypcard.com/), [San Francisco Exploratorium](www.google.com)

## Ingredients
* [Middleman](https://middlemanapp.com/)
* Middleman gems [Middleman S3 Sync](https://github.com/fredjean/middleman-s3_sync) and [Middleman Cloudfront](https://github.com/andrusha/middleman-cloudfront)
* [AWS S3](http://aws.amazon.com/s3/) and [AWS Cloudfront](http://aws.amazon.com/cloudfront/)
* [CircleCI](https://circleci.com/) as a continuous integration platform for deployment to AWS and for automated testing
* [Prismic](https://prismic.io/) for Content Management

**The following are instructions for generating a static site with Middleman, Amazon Web Services, CircleCI and Prismic from scratch.**

## Table of Contents
* [Running the local web server](#web_server)
* [Create a new Middleman Site](#new_middleman_project)
* [Get AWS access keys and Attach a Policy in AWS Identity & Access Management (IAM)](#aws_iam)
* [Setup an AWS S3 Bucket](#aws_s3)
* [Add on Amazon Cloudfront content delivery web service](#aws_cloudfront)
* Prismic: Creating Documents and adding a Webhook with CircleCi
* Launch Day in AWS

<a name="web_server"></a> ### Running the local web server

1. **Bundle Gems**

  <code> bundle install </code>

2. **Compile files**

   <code> bundle exec middleman build </code>

3. **Start a local web server running at: http://localhost:4567/**

  <code> bundle exec middleman </code>

<a name="new_middleman_project"></a> ### Create a new Middleman site

1. Follow steps to [install Middleman](https://middlemanapp.com/basics/install/) and [start a new site](https://middlemanapp.com/basics/start_new_site/)


<a name="aws_iam"></a> ### Grab AWS access keys and Attach a Policy in AWS Identity & Access Management (IAM)

1. After an AWS account has been setup, go to AWS IAM

<a name="aws_s3"></a> ### Setup an AWS S3 Bucket

1. **Create a S3 Bucket**
   Go to Services > S3.  Create a Bucket in S3, add a meaningful name (e.g. myappname-production)
   and region option, e.g. Northern California).

   Once you choose a region, search region codes here:
   http://www.bucketexplorer.com/documentation/amazon-s3--amazon-s3-buckets-and-regions.html

   You will need to add your region property in **config.rb** in the [Setup an AWS S3 Bucket](#aws_s3) step.

2. **Enable Static Website Hosting**
    Go to your bucket and click **Properties**.  Under **Static Website Hosting**, click **Enable website hosting**
    and add **index.html** in Index Document and **error.html** in Error Document. **Save.**



