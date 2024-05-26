=========================================================================

# Question2

-We will be using killercoda free servers for today's practical session:

-Go to the below webpage and sign on with your Github account.   

https://killercoda.com/

=========================================================================

# Time 15: mins 

-Set your time by google searching the below:

-google timer 15 minutes countdown

# Questions:

-Look for and click on docker  and select the scenario - add-or-copy

-or 

 -use the below URL:

https://killercoda.com/docker/scenario/add-or-copy

# Perform the below task
 
================================================================


# 1a: Modify the Dockerfile in the /root directory with below 


=================================
~~~
# Use a base image
FROM ubuntu:latest

# Set metadata for the image
LABEL "Author"="Akin"
LABEL "project"="studio"

# Set environment variables, if required
ENV DEBIAN_FRONTEND=noninteractive

# Install dependencies, if any
RUN apt update && apt install git wget unzip apache2 -y

# Expose any necessary ports
EXPOSE 80

# Set the working directory
WORKDIR /var/www/html

# Set volumes
VOLUME /var/log/apache2

# Download and extract the web application
RUN wget -O mediplus-lite.zip https://www.free-css.com/assets/files/free-css-templates/download/page296/mediplus-lite.zip && \
    unzip mediplus-lite.zip && \
    cd mediplus-lite && \
    cp -r * /var/www/html/ && \
    rm -rf mediplus-lite.zip mediplus-lite

# Define the default command if ENTRYPOINT is present
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]

~~~
=====================================

# Build the docker image and confirm the docker image is build.

 - Hint:
    - docker build -t jendaredocker/mediplus-lite:v6 . 
    - docker images

=====================================

# 1b: Create a running instance of an image called: jendaredocker/mediplus-lite:v6 

  - Hint:

  - docker run -d -it --name mediplus-lite-webpage -p 8000:80 jendaredocker/mediplus-lite:v6
    
  - run the necessary docker commands to show the container is running.

=====================================

# c: Copy and paste the full container ID on the group chat 



===================================================================
===================================================================
