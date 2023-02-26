# Week 1 — App Containerization

## Completed required assignments without issue

## Homework Challenges:
1. Pushed and tagged an image to Dockerhub
- This was my first time tagging and pushing to Dockerhub. I had to read the documentation and watch a YouTube video to learn how to do this but once I did it was very straightforward to do.
- https://hub.docker.com/r/ismarjiw/test/tags

2. Researched best practices of Dockerfiles and implemented a few in my Dockerfile:
- My reference: https://docs.docker.com/develop/develop-images/dockerfile_best-practices/ 
- For example, in the frontend-react-js Dockerfile, as a best practice I have ``COPY`` indicating copying of local files into the container vs. ``ADD`` which isn't as transparent -> ``ADD`` would be best used for local tar file auto-extraction into the image.
- Another best practice in the frontend-react-js Dockerfile is setting ``EXPOSE`` to the ENV PORT=3000 which is the common/traditional port for Node.js appications.