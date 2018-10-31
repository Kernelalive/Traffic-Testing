FROM ubuntu:latest

RUN apt-get update
RUN apt-get install -y nodejs npm 
RUN npm install -g http-server

# Add additional tools
#RUN apt-get install -y nano links git wget curl htop

CMD http-server .
