[![alt text](/README_Images/monsoon_.png)](http://www.monsoonco.com/)

Middleman AWS Prismic CircleCi
=================
Welcome to our Middleman-AWS-Prismic-CircleCi open source project!
We've used this lovely setup for creating these live projects at Monsoon: [LunaSleep](http://lunasleep.com/), [Swypcard](https://www.swypcard.com/), [San Francisco Exploratorium](www.google.com)

## Ingredients
* [Middleman](https://middlemanapp.com/)
* Middleman gems [Middleman S3 Sync](https://github.com/fredjean/middleman-s3_sync) and [Middleman Cloudfront](https://github.com/andrusha/middleman-cloudfront)
* [AWS S3](http://aws.amazon.com/s3/) and [AWS Cloudfront](http://aws.amazon.com/cloudfront/)
* [CircleCI](https://circleci.com/) for continuous integration
* [Prismic](https://prismic.io/) for Content Management

**Instructions for generating a static site with Middleman, Amazon Web Services, CircleCI and Prismic from scratch.**

## Table of Contents
* [Running the local web server](#web_server)
* [Create a new Middleman Site](#new_middleman_project)
* [Get AWS access keys and Attach a Policy in AWS Identity & Access Management](#aws_iam)
* [Setup an AWS S3 Bucket](#aws_s3)
* [Add on Amazon Cloudfront content delivery web service](#aws_cloudfront)
* Deploy to AWS S3 and Cloudfront Setup with CircleCi
* Prismic: Creating Documents
* Prismic Webhook: Trigger a build in CircleCi everytime there's a change in content
* Launch Day in AWS

<a name="web_server"></a> Running the local web server
-------------

1. **Bundle Gems**

  <code> bundle install </code>

2. **Compile files**

   <code> bundle exec middleman build </code>

3. **Start a local web server running at: http://localhost:4567/**

  <code> bundle exec middleman </code>

<a name="new_middleman_project"></a> Create a new Middleman site
-------------

1. Follow steps to [install Middleman](https://middlemanapp.com/basics/install/) and [start a new site](https://middlemanapp.com/basics/start_new_site/)


<a name="aws_iam"></a>Get AWS access keys and Attach a Policy in AWS Identity & Access Management
-------------


<a name="aws_s3"></a> Setup an AWS S3 Bucket
-------------



