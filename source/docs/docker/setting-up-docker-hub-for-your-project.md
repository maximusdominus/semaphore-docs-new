---
layout: post
title: Setting up Docker Hub for your project
category: Docker
---

[Docker Hub](https://hub.docker.com/) is a cloud hosted service for your Docker
images. You can [sign up](https://hub.docker.com/) for an account if you don't
have one already.

Configuring your **Semaphore account** with **Docker Hub** smooth and fast and
it will last a minute of your time.

Project that is set up as a **Docker** project will have Docker container
registry integrations in project add-ons. To set up your project as a Docker
project, please look into
[Setting up a continuous integration for a Docker project on Semaphore](/docs/docker/setting-up-continuous-integration-for-docker-project.html)
page in our documentation.

Configuring the Docker Hub project add-on will enable you to **push** and
**pull** your images without explicitly having to login to Docker Hub during
builds and deployments, thus making your CI and CD process painless.

This can be done by visiting your project on Semaphore and clicking "Add-ons"
at the upper right corner of your screen.

<img src="" class="img-responsive img-bordered" alt="Click Project Add-ons">

Next, click "Docker integrations".

<img src="" class="img-responsive img-bordered" alt="Click Docker integrations">

Choose "Docker Hub" integration.

<img src="" class="img-responsive img-bordered" alt="Click Docker Hub integration">

Then you will be prompted with two input fields requiring your `Username` and
`Password` for Docker Hub. Please input these and test if your credentials are
valid by clicking the "Test" button.

<img src="" class="img-responsive img-bordered" alt="Successful connection test and Save">

If the credentials you provided are valid, click "Save". You can now push or
pull images on Docker Hub through Semaphore.

Happy building!
