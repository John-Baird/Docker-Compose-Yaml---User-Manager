docker build . -f D -t user-manager

docker run -d  --name buster -p 3000:3000 user-manager:latest

Go to http://localhost:3000/users



//Docker Compose Yaml//

docker stack deploy -c docker-compose.yaml user-manager

docker service scale user-manager_service1=7

docker stack rm user-manager 