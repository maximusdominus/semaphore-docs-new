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
at the bottom right corner of your screen.

###### "Add-ons link" screenshot

Next, click "Docker integrations".

###### "Docker integrations" screenshot

Choose "Docker Hub" integration.

###### "Docker Hub integration" screenshot

Then you will be prompted with two input fields requiring
your username and password for Docker Hub. Please input these and test if your
credentials are valid by clicking "Test and Save" button.

###### "Docker Hub credentials" screenshot

If the credentials you provided are valid, your Docker Hub integration will be
saved. You can now push or pull images on Docker Hub through Semaphore.

Happy building!
