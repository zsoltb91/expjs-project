Used commands:

>> node index.js
>> docker build -t expjs-project
>> docker run -p 3000:3000 expjs-project


//To list running docker containers and stop them if needed
>> sudo docker container ls
>> sudo docker rm -f <container name>

//Lists PIDs what uses TCP port 3000
>> sudo lsof -ti:3000