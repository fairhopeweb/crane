<img src="https://raw.githubusercontent.com/InfuseAI/crane/main/public/images/Logo_hori.png" alt="Crane" style="height: 130px;">

[![GitHub release](https://img.shields.io/github/release/infuseAI/crane/all.svg)](https://github.com/infuseAI/crane/releases)
![workflow](https://github.com/InfuseAI/crane/actions/workflows/build.yml/badge.svg?branch=main)
![](https://img.shields.io/badge/Present-InfuseAI-blue)
![](https://img.shields.io/badge/Made%20with-%E2%9D%A4-red)
[![InfuseAI Discord Invite](https://img.shields.io/discord/664381609771925514?color=%237289DA&label=chat&logo=discord&logoColor=white)](https://discord.gg/ZE8pQ8gRWy)

[![](https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=crane)](https://www.producthunt.com/posts/crane)

An easy and beautiful way to manage and build your container images.

Crane helps people building machine-learning notebook container images.

Check [this article](https://medium.com/infuseai/crane-the-minimalist-container-image-builder-68253722be8c) for more initiatives about Crane.

> Like crane? Crane works better with [PrimeHub](http://one.primehub.io/). Crane is the best companion of PrimeHub when it comes to managing docker images. [Try PrimeHub Now](http://one.primehub.io/) and join our [discord community](https://discord.com/invite/ZE8pQ8gRW)!

## Install

Download the latest version from our [releases](https://github.com/infuseAI/crane/releases) page.

## Features

### Building a Container Image

Install packages with apt, conda and pip, which should work in most notebook images. And you can also find a list of our [pre-built container images](https://docs.primehub.io/docs/guide_manual/images-list) in the Base Image dropdown menu.

<img width="1136" alt="CleanShot 2021-10-19 at 02 41 12@2x" src="https://user-images.githubusercontent.com/935988/137788380-f5632f67-a5f4-42fe-b802-da2387cfa41f.png">

### Manage Credentials

Manage your remote registry credentials and PrimeHub API token securely. Now only docker hub is supported. More on the way.

Credentials are stored safely in the Keychain(MacOS), libsecret(Linux) or Credential Vault(Windows).

<img width="1136" alt="CleanShot 2021-10-19 at 03 14 32@2x" src="https://user-images.githubusercontent.com/88208/140909366-7bd2b1cd-6522-4440-98c7-95aa73225da8.png">

### Manage Local And Remote Images

Simple yet informative GUI. For now to manipulate local and remote images.

<img width="1136" alt="CleanShot 2021-10-19 at 02 41 36@2x" src="https://user-images.githubusercontent.com/935988/137788310-d48dc8e9-cc47-479f-95da-5c651129b57f.png">

### Import Remote Image Into PrimeHub

From the Remote Repository list, users can import the image into the connected PrimeHub cluster. This feature only works with public container images for now.

<img width="1136" alt="CleanShot 2021-11-02 at 17 50 15@2x" src="https://user-images.githubusercontent.com/88208/140909656-62c1dbf6-57d9-4743-a83e-7e44ff522b88.png">

## Let's chat about Crane 🦩

**So, what is Crane?**

Crane is a minimalist container image builder. You can extend an existing container image with custom apt/conda/pip packages without writing any Dockerfile.

**How does Crane work?**

Crane generates Dockerfile that installs packages according to your settings, and builds the container image with your local docker engine. You can also push images to your Docker Hub registry.

**Why we built Crane?**

Container images are used in many different use cases such as ML. There are lots of ready-to-run container images with Jupyter and various libraries, however people still want to customize images, and this is mostly done through authoring Dockerfile with commands installing additional packages.

Dockerfile is the canonical way for building container images. However, people still want a no-frills way to just simply adding packages to existing images. Crane provides an easier way to build container images without any knowledge of Dockerfile, so the process is more approachable.

We've always had this feature in our open source ML platform PrimeHub to allow customizing container images for a shared and consistent environment. And it's now also available as a standalone desktop app - Crane. 