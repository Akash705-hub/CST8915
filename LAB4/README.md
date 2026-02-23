# CST8915 Lab 2: Deploying the Algonquin Pet Store on Azure

- **Student Name**: Akash Patel
- **Student ID**: 041269598
- **Course**: CST8915 Full-stack Cloud-native Development
- **Semester**: Winter 2026

---

## Demo Video

🎥 I added the video under over here: Click Here

---

## Technical Explanations

### What are the main differences between a Docker image and a Docker container?
- A Docker image is a read only template which includes application code, runtime, libraries and dependencies required to execute an application whereas a Docker container is a running instance of an image. An image can be described simply as a blueprint or snapshot and a container as the live running environment that has been built out of it. You are able to make numerous containers based on the same image and can be started, stopped and deleted without the original image altering.
### Explain how Docker's layered architecture improves efficiency.
- The architecture of Docker is more efficient since it creates images by creating a reusable layer, meaning that shared elements such as the base operating system and dependencies can be reused on a single image and container. This saves on storage, accelerates image downloading and builds are quicker since it is only the modified layers to be recreated, rather than the full image. It is also better at consistency and version management, as every layer characterizes a particular modification in the application.
### Why does each container get its own writable layer? 
- On top of each container, there is a writable layer to make it isolated and independent. Base image layers are read-only and shared, but the writable layer can be used by a container to write its own runtime changes e.g. logging, temporary files, and modified data, without any impact on the underlying image or any other containers started on the same basis image. This design ensures that there is no overlapping and no conflict between containers, besides ensuring that there is a possibility of many containers operating alongside the same image.
