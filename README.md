[![alt text](/README_Images/monsoon_.png)](http://www.monsoonco.com/)

Middleman AWS Prismic CircleCi
=================



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

