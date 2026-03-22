#1 Install Docker on Ubuntu
  >> sudo apt install gnome-terminal
  >> sudo apt-get update
  >> sudo apt install ./docker-desktop-amd64.deb

#2 Install Jenkins (inside Docker) on Ubuntu
  Create a bridge network called jenkins: >> docker network create jenkins



#3 Already have a running Jenkins server (with docker)
#4 Already have an ExpressJs app running in docker

#5 Let's start a Jenkins build that starts the ExpressJs docker image.


Used commands:

>> node index.js
>> docker build -t expjs-project
>> docker run -p 3000:3000 expjs-project


//To list running docker containers and stop them if needed
>> sudo docker container ls
>> sudo docker rm -f <container name>

//Lists PIDs what uses TCP port 3000
>> sudo lsof -ti:3000