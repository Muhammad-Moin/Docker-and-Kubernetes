Images:

A container images is a lightweight,standalone,executable package of software that includes everything needed to run application.
* code
* Runtime
* System Tool
* System libraries
* Settings

1- Image become container when they run on Docker Engine.
Images is a build time.
Container is a run time.

* Container are all about being fast and lightweight.
* Docker images are stored in image registeries. i.e https://www.dockerhub

Image naming and tagging:
docker image pull <repository>:<tag>
docker image pull nginx:latest

Containerizing an app form scratch.
The process of containerining an app looks like this:
* start with your application code.
* create a Dockerfile that describe your app, its dependancies, and how to run it.
* feed this Dockerfile into the docker image build command to create an image.
* create and run a container from the image.
