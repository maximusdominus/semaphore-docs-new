---
layout: post
title: Setting up Amazon EC2 Container Registry for your project
category: Docker
---

[Amazon EC2 Container Registry](https://aws.amazon.com/ecr/) is a Docker
container registry for easily managing, storing and deploying Docker images.
It comes from a family of [Amazon Web Services (AWS)](https://aws.amazon.com/),
so if you don't already have an Amazon account, you can
[sign up](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html).

Integrating your **Semaphore account** with **Amazon EC2 Container Registry
(ACR)** is quick and painless and it will take a couple of minutes of your
time.

Project that are set up to use **Docker** will have container registry
integrations available as project add-ons. More on how to set up your project
as a Docker project in our documentation page,
[Setting up a continuous integration for a Docker project on Semaphore](/docs/docker/setting-up-continuous-integration-for-docker-project.html).

Configuring the Amazon EC2 Container Registry (ACR) project add-on will enable
you to **push** and **pull** your images without explicitly having to login to
ACR during builds and deployments.

This can be done by visiting your project on Semaphore and clicking "Add-ons"
at the upper right corner of your screen.

<img src="" class="img-responsive img-bordered" alt="Click Project Add-ons">

Next, click "Docker integrations".

<img src="" class="img-responsive img-bordered" alt="Click Docker integrations">

Choose "Amazon EC2 Container Registry (ACR)" integration.

<img src="" class="img-responsive img-bordered" alt="Click Amazon Container Registry (ACR)">

Then you will be prompted with three input fields requiring
your:

  - `AWS Access Key ID`,
  - `AWS Secret Access Key`,
  - `AWS Region` - region where your repository resides.

You can find instructions for managing AWS credentials at
[their documentation](http://docs.aws.amazon.com/general/latest/gr/managing-aws-access-keys.html).
You should also consider making an
It is a good practice to create a new [IAM user](http://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html)
whose purpose will be to interact with Semaphore.

After verifying your credentials with the "Test" button, saving them will
complete the setup process.

<img src="" class="img-responsive img-bordered" alt="Successful connection test and Save">

You can now push or pull images on Amazon Container Registry through Semaphore.

Happy building!
