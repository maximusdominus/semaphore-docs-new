---
layout: post
title: Deploying Docker images to Docker Hub
category: Docker
---

[Docker Hub](https://hub.docker.com/) is a cloud hosted service for your Docker
images. You can effortlessly share Docker images on Docker Hub and make them
public or private. You can [sign up](https://hub.docker.com/) for an account if
you don't have one.

Integrating your **Semaphore account** with **Docker Hub** is very easy and it
will take a minute of your time.

If you haven't set up your project as a **Docker project**, you should consult
[Setting up a continuous integration for a Docker project on Semaphore](/docs/docker/setting-up-continuous-integration-for-docker-project.html)
page in our documentation in order to have Docker integrations available for
your project.

You should definitely set up Docker Hub integration if you are planning on:

  - **pulling Docker images** from a private Docker Hub repository,
  - **pushing Docker images** to Docker Hub.

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
