---
layout: post
title: "Continuous Integration & Deployment of Azure Websites Using Team City and Octopus Deploy"
date: 2015-08-05T14:10:50-07:00
---

# Overview

For the past few years our application has been served well by the good folks at [Cosentry](https://www.cosentry.com/), but as our team grows and technology that simplifies devops improves, we find our selves wanting to move in that direction.

Here begins our journey...

## Current Setup

#### Hardware
* 1 Database Server
* 1 Webserver

#### Application
* .Net MVC Application
* Frontend Code is a mixture of AngularJS & good old fashion html/javascript/jquery.
* Database migrations handled with a home rolled package similar to this: [http://dbup.github.io/](http://dbup.github.io/)

#### Management & Continous Deployment/Integration
* Github for hosting our git repos.
* Jenkins for CI & Build w/ triggers on master / dev branches.


#### Environments

* Production - Used for production.
* Integration - Used for staging.

# Ideal Setup
Using Azures cloud services


* Azure Development App Service
  SQL Server Hosted on Azure
* Azure Production App Service
  SQL Server Hosted on Azure
* TeamCity for Continuous Integration
* OctopusDeploy for Continous Deployments

