# Containerization
Dockerise a rails application

## Tasks completed
- Containerize this rails application using Docker.
- Launch the application in a docker container. Launch a separate container for the database and ensure that the two containers are able to connect.
    - The DB port should not be exposed to the host or external network. It must be internal to the docker network only.
    - Expose the application port to the host machine at port 8080. So you should be able to access the app at “localhost:8080”.
- Use Docker Compose to bring up all services together.
    - Expose only the required services.
- [Bonus] Launch an Nginx container, and configure it as a reverse proxy to the rails application. Expose it at port 8080 on localhost. So now the rails application shouldn’t be accessed directly. All requests will go through Nginx
- [Bonus] Launch two more containers of the rails application. All three containers should be able to connect to a single database container. Configure Nginx container to load balance incoming requests between the three containers.
- [Bonus] Enable persistence for the DB data and Nginx config files so that they are available even when the containers go down. Use docker-compose to easily bring these containers up together with a single command. (half done the storage for file is not shared and is local only one service)


## Erros
- Too many i lost count
