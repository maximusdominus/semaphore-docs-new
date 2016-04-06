---
layout: post
title: Deploying Docker images to Custom Registries
category: Docker
---

[Docker](https://www.docker.com/) brought many good things to the world of
distributed applications and containerization, and one of those thins is an
ability to have **your own private container registries** for Docker images.

Integrating your **Semaphore account** with your **Custom Container Registry**
is very easy and it will take a minute of your time.

If you haven't set up your project as a **Docker project**, you should consult
[Setting up a continuous integration for a Docker project on Semaphore](/docs/docker/setting-up-continuous-integration-for-docker-project.html)
page in our documentation in order to have Docker integrations available for
your project.

You should definitely set up Docker Hub integration if you are planning on:

  - **pulling Docker images** from a custom repository,
  - **pushing Docker images** to a custom repository.

This can be done by visiting your project on Semaphore and clicking "Add-ons"
at the upper right corner of your screen.

<img src="" class="img-responsive img-bordered" alt="Click Project Add-ons">

Next, click "Docker integrations".

<img src="" class="img-responsive img-bordered" alt="Click Docker integrations">

Choose "Docker Hub" integration.

<img src="" class="img-responsive img-bordered" alt="Click Custom Container Registry integration">

Then you will be prompted with three input fields:

  - `Username` - username you were given or set,
  - `Password` - password you were given or set,
  - `Domain` - your custom registry domain.

Please input these and test if your credentials are valid by clicking the
"Test" button.

<img src="" class="img-responsive img-bordered" alt="Successful connection test and Save">

If the credentials you provided are valid, click "Save". You can now push or
pull images to your custom registry through Semaphore.

Happy building!
