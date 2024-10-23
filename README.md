# Voiture App Backend (Spring Boot)

This is the back-end part of the **Voiture App**, built with **Spring Boot** and **Java 21**, and Dockerized for easy deployment. This guide explains how to set up, build, push, and run the back-end.

## Prerequisites

- **JDK 21** installed. You can download it from [here](https://www.oracle.com/java/technologies/javase/jdk21-archive-downloads.html).
- **Docker** installed. You can get Docker [here](https://www.docker.com/get-started).
- **Maven** installed. Find installation instructions [here](https://maven.apache.org/install.html).
- A **GitHub account** for cloning the repository and pushing updates.
  
## Setup and Build Instructions

### 1. Clone the Repository

   First, you need to clone this repository from GitHub and navigate into the project directory:
   
   - git clone https://github.com/ChakraHs/SpringDataRest-React.git
   - cd voiture-app-backend

### 2. Build the Docker Image

The back-end image is built using **Maven** and the **Spring Boot** plugin. To create the Docker image, run the following command:

- mvn clean package -Pbuild-image

This command will generate a Docker image for the back-end.

### 3. Run Docker Compose

Run the following command to start the the project services using Docker Compose:

- docker compose up -d

This will start all services defined in your `docker-compose.yml`.

## Accessing the Application

Once the services is running, you can access the App at: localhost:3000




