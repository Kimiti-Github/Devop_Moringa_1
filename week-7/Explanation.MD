Base images
Backend And Client Base Image
node:19-alpine - Alpine is much smaller than most distribution base images and thus leads to much slimmer images in general.

Database
mongo - The only available image for Mongo DB

Dockerfile directives
Directive	what-it-does
FROM	This is used to specify the parent image of our custom Docker image
WORKDIR	The WORKDIR instruction sets the working directory for any RUN, CMD, ENTRYPOINT, COPY and ADD instructions that follow it in the Dockerfile
RUN	used to execute commands during the image build time
COPY	The COPY instruction copies new files or directories from and adds them to the filesystem of the container at the path
EXPOSE	informs Docker that the container listens on the specified network ports at runtime
CMD	used to provide this default initialization command that will be executed when a container is created from the Docker image



Naming images and containers
Named the images and containers to make them easy to indentify as below



Link to Docker Hub
https://hub.docker.com/repositories/jwaigwa



Running the Service successfully
I was able to run the services successfully on docker as shown in below images

Running containers

Alt text

Frontend Alt text


Backend API Call
