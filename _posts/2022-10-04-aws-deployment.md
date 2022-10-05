---
toc: true
layout: post
description: AWS Deployment of personal flask
categories: [markdown]
title: AWS Deployment
---

# Docker

We created 4 containers with each site in one of the containers bound to 8080 with their own unique ports.

![]({{site.baseurl}}/images/docker container list.png "https://github.com/fastai/fastpages")

# Docker Compose File

Inside this file is instructions to build container that contain personal flask.

![]({{site.baseurl}}/images/docker compose file.png "https://github.com/fastai/fastpages")

# Nginx



![]({{site.baseurl}}/images/nginx.png "https://github.com/fastai/fastpages")

# cURL Command

Tests if the personal flask is working on local machine

![]({{site.baseurl}}/images/curl better.png "https://github.com/fastai/fastpages")