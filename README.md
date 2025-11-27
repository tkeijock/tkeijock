## Welcome to My Learning Journey with Container, CI/CD

This space documents my continuous progression in mastering Docker, container best practices, and CI/CD automation using GitHub Actions.
Each repository represents a step forward in learning how to design, improve, and automate container-based workflows.


### 📁 1. Dockerfile Best Practices :  

https://github.com/tkeijock/dockerfile-best-practices

This repository focuses on writing Docker files that are efficient, secure, and maintainable.

Here, I explored:  Layer optimization , Caching strategies , Reducing image size and attack surface , Production-ready build patterns
This was the foundation for understanding how containers should be built correctly.

### 📁 2. Pipeline for Docker Image Build & Push

 https://github.com/tkeijock/pipeline-docker
 
This repository introduces a GitHub Actions workflow that: Builds Docker images directly from a Docker file inside its own repository.
Tags them automatically , Pushes them to Docker Hub , Implements build-layer caching for faster builds
The goal was to automate and have a online method to build images and put on a container registry.

### 📁 3. Reusable Docker Build Action (WIP)
(in progress — upcoming repository)

The next step is to transform the previous pipeline-docker into a reusable GitHub Action.
This allows multiple projects to share the same build/push logic without duplicating workflows.

This step generalizes the CI/CD logic, turning it into a plug-and-play action for any project that needs Docker builds.

Planned features:
Accept inputs such as  Docker file , docker hub repo name and final image name.
Build and push container images using a centralized pipeline
Improve maintainability across multiple repositories
