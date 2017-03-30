FROM ubuntu

MAINTAINER Abhinav Saxena

# Install Nginx

# Add application repository URL to the default sources

RUN echo "deb http://archive.ubuntu.com/ubuntu/ raring main universe" >> /etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y nano wget dialog net-tools
RUN apt-get install -y nginx  

# Append "daemon off;"
 
RUN echo "daemon off;" >> /etc/nginx/nginx.conf

EXPOSE 80

CMD service nginx start

     


