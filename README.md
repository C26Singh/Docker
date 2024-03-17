# Docker  
Docker is a platform that allows developers to package, distribute, and run applications and their dependencies in isolated containers.
## Table of Contents

- [Container](#container)
- [What problems does it solve?](#what-problems-does-it-solve)
- [Container repository](#container-repository)
- [Develop application](#develop-application)
- [Deploy application](#deploy-application)

## Container
- A way to package application with all the dependencies and configuration.  
- portible artifacts
- Built of layers of images and configuration data Like-  
  postgres image <-----redis Image <------  ..... <----------Linux base Image
- How to use docker container?  
  docker run | pull postgres:6.6  
  docker ps-->list all images  
  Image --->artifacts.  
  container--->running.  

- Can we run multiple version of an image?  
  yes, and you can run in different container (each container has its own uniqueId)
- Next  
  How to use these container in application?  
  How to do Port configuration?

## Container repository
- private repository
- public repository---------->Docker Hub
## Develop application
- **Before**:
  - Most of the services you need to install on the OS directly.
  - MS SQL Server, PostgreSQL, Redis...

- **After**:
  - No need to directly install services on the OS.
  - Container has its own isolated OS layer.

## Deploy application
- **Before**:
  - Most of the services you need to install on the OS directly.
  - MS SQL Server, PostgreSQL, Redis...

- **After**:
  - No need to directly install services on the OS.
  - Container has its own isolated OS layer.
## Docker vs Virtual Machine  
     Hardware
  +------------------------+  
  |        CPU | Memory     |  
  +------------------------+  
              |  
              v  
         OS Kernel  
  +------------------------+   
  |       Operating        |  
  |       System           |  
  +------------------------+  
              |  
              v  
         Application  

 - both are virtualization tools  
  - **What part do they virtualise?**
     - Docker Virtualisez the Application layer.
     - VM virtualize (OS Kernal+Application)
     - compatibility-->  
        VM image of any OS run on any OS host.  
        but can not do that with Docker.
    - What is the problem docker?  
      Want to run linux based image on windows based host

      Windows(Host)  
      VM Linux------->will work  
      Docker Linux---> not compatible for Windows OS kernal.  
      For windows version below 10---> use docker toolbox to abstract kernal so it can work with different docker images.
 ## Installation  
   pre-requisite
   - Windows -->download the installer.
   - windows version is compatible
   - Virtualization enabled.


   - **What docker Installer brings to your system?**
   - Docker Toolbox-->workaround for older version that do not support running docker natively.
   - Docker cli------>is used to manage  Docker containers and  containerized applications using a set of intuitive commands.
   - Docker Machine-->tool used to create|manage|deploy docker host on VM | Cloud providers
   - Docker compose--> tool for defining and running multi-container Docker applications. Allow users to specify services, networks, and volumes required for an application in a single YAML file
   - Kitematic------->GUI tool provided by Docker to simplify the management of Docker containers and images, allowing users to easily search, download, and manage Docker applications
   - Orcale VM Virtualbox->Oracle VM VirtualBox is a powerful, open-source virtualization software that enables users to run multiple operating systems simultaneously on a single physical machine

      
       
   

