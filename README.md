# EMart Microservice Application

## Overview
EMart is an e-commerce application designed using microservices architecture. This project showcases the deployment of multiple microservices, including a frontend application and backend APIs, utilizing Docker and Docker Compose.

## Architecture
The EMart application consists of the following components:
- **Frontend**: Built with Angular, serving as the client application.
- **API Gateway**: Managed by Nginx, routing requests to the appropriate services.
- **Backend Services**:
  - **Node.js API**: Serves the `/api` endpoint and connects to a MongoDB database.
  - **Java Books API**: Serves the `/web-api` endpoint and connects to a MySQL database.
  
## Features
- User registration and login functionality.
- Product listing from the Java Books API.
- Scalable architecture allowing easy addition of new services.

## Prerequisites
- [Docker](https://www.docker.com/) installed on your machine.
- [Docker Compose](https://docs.docker.com/compose/) for managing multi-container applications.
- [Vagrant](https://www.vagrantup.com/) for VM management (optional).

## Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/hariravendran/EMart-Dockerized-Microservices-E-Commerce-Solution
```bash

(Unzip)
```bash
cd EMart```bash

2. Set Up the Environment
Ensure that your Vagrant VM is powered off before starting.

bash
vagrant up
vagrant ssh
3. Build and Run the Application
Navigate to the project directory and build the Docker containers:

bash
docker-compose up -d
If you encounter any issues, you can build the images first:

bash
docker-compose build
docker-compose up -d

4. Access the Application
Open your web browser and go to:http://<your-vm-ip>

5. User Registration and Login
Register a new user by clicking on the register link.
Enter the required information and submit the form.
Log in with the registered credentials to access the product listing.

Cleanup
To stop and remove all containers, run:

bash
docker-compose down
docker system prune -a
Exit from the VM:

bash
exit
And power off the VM:

bash
vagrant halt
Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
Inspired by e-commerce platforms like Amazon and Flipkart.
Built with modern technologies including Angular, Node.js, and Java.
