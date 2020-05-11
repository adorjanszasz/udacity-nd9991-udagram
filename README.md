# udacity-nd9991-udagram

Udacity Cloud DevOps Engineer Nanodegree Program - IaC Project: High-availability web app

## Problem

Your company is creating an Instagram clone called Udagram. Developers pushed the latest version of their code in a zip file located in a public S3 Bucket.

You have been tasked with deploying the application, along with the necessary supporting software into its matching infrastructure.

This needs to be done in an automated fashion so that the infrastructure can be discarded as soon as the testing team finishes their tests and gathers their results.

## Architecture diagrams

#### With bastion

![](/images/Udagram Architecture.jpeg)

#### Without bastion - implemented version

In this case the maintenance is done over SSM without using any SSH keys

![](/images/Udagram_Architecture_bastion_free.jpeg)

## Deployment steps

Deployment steps:

In the AWS CloudFormation console, launch one of the following templates to build a new stack:

- final-project (to deploy both a new VPC and web servers)
- vpc-base.tempate (to deploy a new VPC)
- udagram-servers.template (to deploy the web serverss into your existing VPC)

Use can use the parameter file final-project-params.json as a default setup.
