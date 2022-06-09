# Microservices-using-Docker

## Group Members

- ##### Nurrdinan Serena binti Amer Shariffudin [2012998]
- ##### Nur Zulfah Insyirah binti Fadzleey [2015384]
- ##### Nurhanis binti Abdul Razak [2019214]
- ##### Amirul Azim bin Amran [2017425]

--------

***INTRODUCTION***

Before Docker, developers and testers in the programming industry had a difficult time transporting data between environments. This presents a number of challenges as well as drawbacks for the developer and tester. How to overcome this problem? 

Introducing Docker is one of the solutions. Docker can be thought of as a tool that optimizes the deployment of applications in lightweight containers, allowing them to run efficiently in a variety of environments. By definition, a container is a software package that includes all of the requirements needed to run an application.

For instance, if a chalet has four bedrooms but only one of them has a toilet, this could be a problem because the guests will not have convenient access to the toilet. This is where Docker steps in to help address the issue. To ensure that each room is comfortable, the owner must install a toilet in each room. In this example, toilet refers to the framework. By including a framework in every software application (room), the application will run more smoothly. Thus, Docker will assist in running the application with the appropriate framework.

When compared to virtual machines, Docker has a number of advantages. One of them is Docker, which is lighter than virtual machines but still provides the same functionality. In addition, as compared to virtual machines, Docker consumes less RAM and requires a faster application boot-up time. Apart from that, Docker has a slightly higher efficiency because it is freely accessible across multiple platforms. Finally, the Docker environment provides superior and consistent performance.

To understand how Docker works, we must first look at Docker Engine, which is one of the most important components of Docker. It is a base engine that is installed on the host machine and is used to construct and run docker containers (applications). This is an image of the Docker Engine:
<div align="center">

![ezgif com-gif-maker](https://user-images.githubusercontent.com/93330469/172448562-30be5c47-0f4d-4cbf-8e52-238aca679712.jpg)

</div>
The Docker Client and Server is the first component to look at while looking at the Docker Components. It's a service that sends a command to the containers after it's been translated using REST API (server). The server will examine the client's request and the operating system's answer. This is for creating or managing the app. The next step is to create Docker Containers using Docker Images, which is a template with instructions. Docker Hub or Repository will be used to store the images. The Docker Container, which is a standalone, executable software application, is the third component. The packages comprise applications and their dependencies that can share the same operating system and execute numerous docker containers in the same infrastructure.

The Docker Registry, which is an open source server-side service, is the last but not least. Docker Registry is a service that hosts and distributes Docker images. Images can be placed here not only in public repositories, but also in private repositories. Here's a visual representation of the Docker Components to help understand them better:

<div align="center">
  
![photo1654622504](https://user-images.githubusercontent.com/93330469/172448337-3842bce3-9643-4764-99c4-ab2250c4caf1.jpeg)
  
</div>


-------

***Installation of Docker & Procedures***

A PHP application requires the installation of many environments in order to run the PHP scripts. One of the servers that will allow us to execute the PHP-driven website is MYSQL Database. Each group of applications can be set up to run as a microservice using Docker. The single YML file configures the MYSQL database and PHP Apache, as well as isolating all of the services required by the application.

In order to install Docker, these are the steps and procedures that need to be done in a Microsoft operating system;




**1. Install Docker for macOS**

- Go to Docker Desktop website and download the version of macOS. (https://www.docker.com/products/docker-desktop/)

- Once the download is completed, double-click the DMG file to start installing Docker Desktop on macOS.

<div align="center">

  <img width="866" alt="web page" src="https://user-images.githubusercontent.com/93330469/172763840-d63ea1a8-98d7-4614-8114-bb3bcfa3e35a.png">

</div>

- Then, it will show options to move the Docker to Applications.

<div align="center">

<img width="783" alt="transfer file" src="https://user-images.githubusercontent.com/93330469/172764024-24bb3916-71b9-47eb-a2ec-ae09927347aa.png">

</div>

- Drag the Docker Icon to the Applications directory.

- To launch the Docker Desktop on macOS, double-click the Docker Icon.

<div align="center">

<img width="723" alt="Screenshot 2022-06-09 at 12 27 42 PM" src="https://user-images.githubusercontent.com/93330469/172764172-3e8be7c0-a621-4737-8c4a-decc292a1894.png">

  </div>

- Click **Open Button** to lauch Docker Desktop and **OK Button**. 

- Enter the password and click **Install Helper Button**. After that, the installation of Docker Desktop on macOS is completed.






**2. Install PHP and Apache Web Server**

- Create a directory to store the new project files. To create the file, type **docker-compose.yml** at the root of the new project.

<div align="center">
  <img width="692" alt="yml file" src="https://user-images.githubusercontent.com/93330469/172764476-cf663aab-06a5-4032-a7d4-a674053df3a8.png">

</div>

- Create also two directories within the docker directory i.e php and apache.

<div align="center">
  <img width="693" alt="dockerfile (php)" src="https://user-images.githubusercontent.com/93330469/172764516-eb31758e-ce39-45f5-9626-0f9789d49f80.png">
<img width="682" alt="dockerfile (apache)" src="https://user-images.githubusercontent.com/93330469/172764530-23118c2b-accb-43ec-a0f3-97790ecf9128.png">

</div>

- Create the index.php file within the src directory.

<div align="center">
  <img width="690" alt="indexphp (src)" src="https://user-images.githubusercontent.com/93330469/172764551-21983557-8d43-48db-9504-897b00543191.png">

</div>

- Then, configure the Virtual Host to pass the PHP requests to PHP-FPM vial port 9000. The default configuration is shown below;


<div align="center">
<img width="693" alt="virtual host" src="https://user-images.githubusercontent.com/93330469/172764617-28916858-df59-43d7-8677-08078403cd0b.png">
  
</div>

- Update the Dockerfile within the Apache directory.

<div align="center">
<img width="689" alt="update dockerfile (apache)" src="https://user-images.githubusercontent.com/93330469/172764650-38382cc7-5c77-467f-8032-cc52c7dc9b6e.png">
  
</div>

- Now, run the command docker-compose build to build the images for PHP and Apache Web Server.

<div align="center">
  
 <img width="562" alt="Screenshot 2022-06-09 at 12 53 18 PM" src="https://user-images.githubusercontent.com/93330469/172767381-561950c8-6eaf-424e-b1b9-1d36b63e5d56.png">

</div>

- After completed, run the application using command shown below;

<div align="center">
  
  <img width="564" alt="Screenshot 2022-06-09 at 12 54 32 PM" src="https://user-images.githubusercontent.com/93330469/172767401-5eaa727f-bb07-4ca0-a733-bdce70654f57.png">

</div>

- Open the browser and enter the URL (http://localhost/index.php). 

- Press Ctrl + C to stop the containers.

- The installation completes.




**3. Install MySQL and PHPMyAdmin**

- Update the **docker-compose.yml**

- Run the command docker-compose build to build the application.

- Then, run the command **docker-compose up** to launch the application.

- Try to access PHPMyAdmin from the browser using URL (http://localhost:8085).

- Login to PHPMyAdmin using the username as root and the root password configured in the docker-compose.yml.

- Press Ctrl + C to stop the containers.

- Then, install the PHP extensions to access MySQL from the PHP source files by updating the Dockerfile.

- Run the build and up commands to build the application again and launch it.

- Open the PHP file using the URL (http://localhost/mysql.php).

- Press Ctrl + C to stop the containers.

- The installation completes.
