---
layout: post
title: Deploying Docker images to Google Container Registry
category: Docker
---

[Google Container Registry](https://cloud.google.com/container-registry/) is
a private Docker container registry for storing, fast scalable retrieving
and deploying Docker images. In order to try and use **Google Container
Registry (GCR)** [Google account](https://accounts.google.com/signup) is
needed.

Integrating your **Semaphore account** with **Google Container Registry (GCR)**
is very easy and it will take a couple of minutes of your time.

If you haven't set up your project as a **Docker project**, you should consult
[Setting up a continuous integration for a Docker project on Semaphore](/docs/docker/setting-up-continuous-integration-for-docker-project.html)
page in our documentation in order to have Docker integrations available for
your project.

You should definitely set up Google Container Registry integration if you
are planning on:

  - **pulling Docker images** from GCR repository,
  - **pushing Docker images** to GCR repository.

In order to get needed data for GCR integration you need to:

  1. Visit [Google Developers Console](https://console.developers.google.com/)

  2. Choose a project you want to integrate with Semaphore

  <img src="/docs/assets/img/docker/deploying-docker-images-to-google-container-registry/select-project.png" class="img-responsive img-bordered">

  3. Click "Permissions" in a menu on the left

  <img src="/docs/assets/img/docker/deploying-docker-images-to-google-container-registry/select-permissions.png" class="img-responsive img-bordered">

  4. Go to "Service accounts" and click "Create service account"

  <img src="/docs/assets/img/docker/deploying-docker-images-to-google-container-registry/click-create-service-account.png" class="img-responsive img-bordered">

  5. Type in a meaningful name to you, we named it _Semaphore_ since we are making
  an integration with Semaphore. Then tick "Furnish a new private key" and
  leave "JSON" selected. Finally click "Create" and public/private key JSON
  file will be saved to your disk.

  <img src="/docs/assets/img/docker/deploying-docker-images-to-google-container-registry/create-service-account.png" class="img-responsive img-bordered">

Save this file somewhere safe because you won't be able to retrieve it again from
the Google Console.

Then visit your project on Semaphore and click "Add-ons" at the upper right
corner of your screen.

###### "Add-ons link" screenshot

Next, click "Docker integrations".

###### "Docker integrations" screenshot

Choose "Google Container Registry (GCR)" integration.

###### "Google Container Registry (GCR)" screenshot

Then you need to copy contents of downloaded JSON file from Google Console
which we downloaded in earlier steps.

###### "Google Container Registry (GCR) JSON file" screenshot

After you have copied contents, you can click "Test" to see if everything is
OK. If the test is successful you can click "Save".

###### "GCR credentials" screenshot

If the credentials you provided are valid, your GCR integration will be
saved. You can now push or pull images on Google Container Registry through
Semaphore.

Happy building!
