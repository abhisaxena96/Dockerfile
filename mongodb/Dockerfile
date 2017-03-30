FROM ubuntu

MAINTAINER Abhinav Saxena

# Install MongoDB

# Begin Installation

RUN apt-get update
RUN apt-get install -y mongodb-server
RUN rm -v /lib/systemd/system/mongodb.service 

# Copy a configuration file 
ADD mongodb.service /lib/systemd/system/

CMD systemctl daemon-reload
CMD systemctl start mongod
CMD systemctl start mongod
