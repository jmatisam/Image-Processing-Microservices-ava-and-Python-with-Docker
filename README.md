# Getting Started

## Project Overview. Introduction

This project aims to create a web application using Spring Boot for the frontend and a Python service for image processing. Docker will be used to containerize both the Java application and the Python service, ensuring that they run in isolated environments with the specified versions of JDK and Python.

Components

Java Application Spring Boot:

A web application built with Spring Boot
Handles user interactions and frontend operations
Sends image files to the Python service for processing
Displays the processed images for the user to download or delete

Python Service:

A backend service built with Flask
Processes images by applying face detection and blurring
Returns the processed images to the Java application

Docker:

Containerizes both the Java application and the Python service
Ensures that the Java application runs with JDK 11
Ensures that the Python service runs with Python 3.9
Facilitates the deployment and management of both services using Docker Compose


## Execution. Key Steps
Docker Installation:
Install Docker on the host machine to run containerized applications

Create a Spring Boot project:
Using Spring Initializr with Maven
Add necessary dependencies and structure the project

Docker:
Create Dockerfiles for both the Java application and Python service to define the build process and runtime environment

Docker Compose Configuration:
Create a docker-compose.yml file to manage and run both services together

Running the Containers:
Build and run the Docker containers using Docker Compose
Running the Project
Navigate to the project root directory
Run docker-compose up --build to build and start the containers

Access the Java application at http://localhost:8080 and the Python service at http://localhost:5000
By using Docker, this project ensures consistency in development and deployment environments, making it easier to manage dependencies and run the application across different systems.


### Reference Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/3.3.0/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/3.3.0/maven-plugin/reference/html/#build-image)
* [Thymeleaf](https://docs.spring.io/spring-boot/docs/3.3.0/reference/htmlsingle/index.html#web.servlet.spring-mvc.template-engines)
* [Spring Web](https://docs.spring.io/spring-boot/docs/3.3.0/reference/htmlsingle/index.html#web)
* [Docker](https://www.docker.com/support/)
* [Python](https://www.python.org/doc/)

### Guides
The following guides illustrate how to use some features concretely:

* [Handling Form Submission](https://spring.io/guides/gs/handling-form-submission/)
* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)
* [mtcnn-opencv 1.0.2](https://pypi.org/project/mtcnn-opencv/)



