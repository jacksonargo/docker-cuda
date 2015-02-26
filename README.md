# docker-cuda

Cuda
====
An automated docker build for a full cuda environment

#### Table of Contents
1. [Description](#desctiption)
2. [Usage](#usage)
3. [Bugs](#bugs)
4. [Authors](#authors)

## Description

This is a Docker image for building cuda code. The nvidia drivers and cuda compiler are installed from the nvidia cuda repos. This image is monster in size, but it has all the build tools needed.

The tag 'latest' and the tag '6.5' are the same right now. Whenever a new cuda version is released, I'll update the 'latest' tag and keep '6.5' using cuda6.5. 

## Usage

You can check the version of the cuda compiler using:

    docker run --rm jacksonargo/cuda:6.5 /usr/local/cuda/bin/nvcc -V

If you want to run cuda code, you don't need the entire build environment and can grab a lighter Docker image
that only contains the nvidia driver such as https://registry.hub.docker.com/u/jacksonargo/nvidia.

## Bugs
If you find any bugs or want to recommend features, send an email to jackson@jacksonargo.com

## Authors
* Jackson Argo
