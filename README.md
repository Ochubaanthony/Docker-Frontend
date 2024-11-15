# Docker-Frontend
Running a container for Frontend docker

FRONTEND DOCKERFILE

GO TO THE SAME  TERMINAL AND RUN THIS

PASTE THE Frontend react repo
git clone https://github.com/soundn/CICD-react-frontend.git




ls
cd CICD-react-frontend
nano Dockerfile
cat Dockerfile

docker build -t front .

Run the Container
docker run -d front:latest

docker image ls
docker ps
docker stop b1d4dd4b696c
docker run -d -p 5173:5173 front:latest

CONFIRM THE PORT 
http://72.144.246.77:5173/

docker ps
docker logs 3922635f9b7c (this is the container ID)
docker stop 3922635f9b7c






HOW TO PULL AN IMAGE
docker ps
docker run -d -p 3000:5173 tonymore/vivianwebapp:T1.0.0
docker ps

USED THIS TO REMOVED ALL CONTAINERS
docker system prune
docker image ls
docker image rm tonymore/vivianwebapp
