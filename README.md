# docker-examples
- https://docs.google.com/presentation/d/11FjKkTkWjLUD6SfrMjrLERcegDgFXiy-Np7QnYf4Gu4/edit?usp=sharing

# docker
- Commands:
    - docker ps
    - docker run
    - docker pull alpine
    - docker run -it  alpine:3.7 sh —> ejecuta un nuevo contenedor
    - docker exec -it [container ID] —> ejecuta un comando dentro de un contenedor que ya esta corriendo
    - docker ps -a | head —> obtiene los últimos 10 contenedores
    - docker image tag [id contenedor] [Nombre del tag]
    - docker stop [id contenedor] —> detener el contenedor
    - docker rm [id contenedor] —> eliminar el contenedor
    - docker rm -f [id contenedor]
    - docker start [id contenedor  id contenedor]
    - docker stop `docker ps -q`   —> detener todos los contenedores
    - docker exec -it [id contenedor] bash

- Examples:
```bash
$docker pull redis
$docker run --name local-redis -p 6379:6379  -d redis 
$docker exec -it local-redis redis cli
```
# dockerfile
- Commands:
    - docker build -t first-dockerfile -f Dockerfile1 .
    - docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
        - ej: docker run -it  -p 3070:3070 docker-demo-10 index.js
    - docker exec -it [id_contenedor] [command]

# docker-compose
- Commands:
    - docker compose --help
    - docker compose up
    - docker compose up -d
    - docker compose stop
    - docker compose down
    - docker compose ps
    - docker compose ps -a

