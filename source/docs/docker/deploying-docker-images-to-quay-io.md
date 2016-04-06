---
layout: post
title: Deploying Docker images to Quay.io
category: Docker
---

[Quay.io](https://quay.io/) is a cloud hosted service for your Docker images.
Focus is on user experience for developers that are pushing and pulling images
from **Quay.io**. If you don't own an account at Quay.io, you can
[try it for free](https://quay.io/plans/?trial-plan=free).

Integrating your **Semaphore account** with **Quay.io** is very easy and it
will take a minute of your time.

If you haven't set up your project as a **Docker project**, you should consult
[Setting up a continuous integration for a Docker project on Semaphore](/docs/docker/setting-up-continuous-integration-for-docker-project.html)
page in our documentation in order to have Docker integrations available for
your project.

You should definitely set up Quay.io integration if you are planning on:

  - **pulling Docker images** from Quay.io registry,
  - **pushing Docker images** to Quay.io registry.

This can be done by visiting your project on Semaphore and clicking "Add-ons"
at the upper right corner of your screen.

<img src="" class="img-responsive img-bordered" alt="Click Project Add-ons">

Next, click "Docker integrations".

<img src="" class="img-responsive img-bordered" alt="Click Docker integrations">

Choose "Quay.io" integration.

<img src="" class="img-responsive img-bordered" alt="Click Quay.io integration">

Then you will be prompted with three input fields:

  - Quay.io `Username`,
  - Quay.io `Password`,
  - Quay.io `Email address`.

Please input these and test if your credentials are valid
by clicking the "Test" button.

<img src="" class="img-responsive img-bordered" alt="Successful connection test and Save">

If the credentials you provided are valid, click "Save". You can now push or
pull images on Quay.io through Semaphore.

Happy building!
