#Installing Jenkins with Docker Compose
This repository provides a Docker Compose configuration for quickly setting up Jenkins. Please note, this setup is not designed for production environments.

Credits: This method is primarily based on the official documentation, but simplifies the process by utilizing Docker Compose (docker-compose.yml) to minimize setup steps.

#Docker Installation
#Step 1: Install Docker
Start by installing Docker on your system. Using Docker Desktop is likely the easiest option.

#Step 2: Clone or Download the Repository
Clone this repository or download its contents to your local machine.

#Step 3: Build the Jenkins Docker Image
In a terminal window, navigate to the directory where this repository's Dockerfile is located. Then, build the Jenkins image with the following command:

```
docker build -t my-jenkins .
```

#Step 4: Start Jenkins
To start Jenkins, run:
```
docker compose up -d
```

#Step 5: Access Jenkins
Once Jenkins is running, open your browser and go to: http://localhost:8080/ to complete the installation.

#Step 6: Stopping Jenkins
If you'd like to stop Jenkins and resume later, run the following command:
```
docker compose down
```
To restart Jenkins later, simply run the same command from Step 4.

#Removing Jenkins
When you're done using Jenkins and want to clean up, you can remove it and all associated resources by running:

```
docker compose down --volumes --rmi all
```
