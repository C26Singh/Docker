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
- Built of layers of images Like-  
  postgres image <-----redis Image <------  ..... <----------Linux base Image

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
