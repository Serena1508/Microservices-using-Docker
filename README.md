# Microservices-using-Docker

## Group Members

- ##### Nurrdinan Serena binti Amer Shariffudin [2012998]
- ##### Nur Zulfah Insyirah binti Fadzleey [2015384]
- ##### Nurhanis binti Abdul Razak [2019214]
- ##### Amirul Azim bin Amran [2017425]

--------

**1. INTRODUCTION**

Before Docker, developers and testers in the programming industry had a difficult time transporting data between environments. This presents a number of challenges as well as drawbacks for the developer and tester. How to overcome this problem? 

Introducing Docker is one of the solutions. Docker can be thought of as a tool that optimizes the deployment of applications in lightweight containers, allowing them to run efficiently in a variety of environments. By definition, a container is a software package that includes all of the requirements needed to run an application.

For instance, if a chalet has four bedrooms but only one of them has a toilet, this could be a problem because the guests will not have convenient access to the toilet. This is where Docker steps in to help address the issue. To ensure that each room is comfortable, the owner must install a toilet in each room. In this example, toilet refers to the framework. By including a framework in every software application (room), the application will run more smoothly. Thus, Docker will assist in running the application with the appropriate framework.

When compared to virtual machines, Docker has a number of advantages. One of them is Docker, which is lighter than virtual machines but still provides the same functionality. In addition, as compared to virtual machines, Docker consumes less RAM and requires a faster application boot-up time. Apart from that, Docker has a slightly higher efficiency because it is freely accessible across multiple platforms. Finally, the Docker environment provides superior and consistent performance.

To understand how Docker works, we must first look at Docker Engine, which is one of the most important components of Docker. It is a base engine that is installed on the host machine and is used to construct and run docker containers (applications). This is an image of the Docker Engine:

![ezgif com-gif-maker](https://user-images.githubusercontent.com/93330469/172448562-30be5c47-0f4d-4cbf-8e52-238aca679712.jpg)

The Docker Client and Server is the first component to look at while looking at the Docker Components. It's a service that sends a command to the containers after it's been translated using REST API (server). The server will examine the client's request and the operating system's answer. This is for creating or managing the app. The next step is to create Docker Containers using Docker Images, which is a template with instructions. Docker Hub or Repository will be used to store the images. The Docker Container, which is a standalone, executable software application, is the third component. The packages comprise applications and their dependencies that can share the same operating system and execute numerous docker containers in the same infrastructure.

The Docker Registry, which is an open source server-side service, is the last but not least. Docker Registry is a service that hosts and distributes Docker images. Images can be placed here not only in public repositories, but also in private repositories. Here's a visual representation of the Docker Components to help understand them better:

![photo1654622504](https://user-images.githubusercontent.com/93330469/172448337-3842bce3-9643-4764-99c4-ab2250c4caf1.jpeg)
