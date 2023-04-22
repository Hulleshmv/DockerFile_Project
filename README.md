# DockerFile_Project

Write a docker file to setup a nginx server

# Nginx Dockerfile

This Dockerfile sets up an Nginx server in a Docker container.

# Usage

To build the Docker image, run the following command in the same directory as the Dockerfile:

docker build -t my-nginx-server .

This will build the Docker image and tag it with the name `my-nginx-server`.

To start a container from the image, run the following command:

docker run -d -p 80:80 -p 443:443 my-nginx-server

This will start a detached container and map ports 80 and 443 on the host to the corresponding ports on the container.

# Customization

You can customize the Nginx server configuration by editing the `nginx.conf` file in the same directory as the Dockerfile. 

When building the Docker image, this file will be copied to the `/etc/nginx` directory in the container, overwriting the default configuration file.
