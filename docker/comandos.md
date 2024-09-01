### 1. Comandos Básicos

- **_docker --version:_** Mostra a versão do Docker instalada.
- **_docker info:_** Exibe informações detalhadas sobre o sistema Docker.
- **_docker help:_** Lista todos os comandos disponíveis no Docker.

### 2. Imagens

- **_docker images:_** Lista todas as imagens locais.
- **_docker pull <imagem>:_** Faz o download de uma imagem do Docker Hub ou de outro registro.
- **_docker build -t <nome>:<tag> .:_** Constrói uma imagem a partir de um Dockerfile na pasta atual.
- **_docker tag <imagem> <novo_nome>:<nova_tag>:_** Marca uma imagem com um novo nome ou tag.
- **_docker rmi <imagem>:_** Remove uma imagem local.
- **_docker save -o <arquivo.tar> <imagem>:_** Salva uma imagem em um arquivo tar.
- **_docker load -i <arquivo.tar>:_** Carrega uma imagem a partir de um arquivo tar.

### 3. Containers

- **_docker ps:_** Lista todos os containers em execução.
- **_docker ps -a:_** Lista todos os containers, incluindo os que não estão em execução.
- **_docker run <imagem>:_** Cria e inicia um novo container a partir de uma imagem.

##### Exemplo: docker run -d -p 8080:80 <imagem> (Executa o container em segundo plano e mapeia a porta 8080 para a 80).

- **_docker start <container>:_** Inicia um container parado.
- **_docker stop <container>:_** Para um container em execução.
- **_docker restart <container>:_** Reinicia um container.
- **_docker rm <container>:_** Remove um container.
- **_docker logs <container>:_** Exibe os logs de um container.
- **_docker exec -it <container> <comando>:_** Executa um comando em um container em execução.

##### Exemplo: docker exec -it <container>\*\*\* /bin/bash (Acessa o shell do container).

### 4. Volumes

- **_docker volume create <nome>:_** Cria um novo volume.
- **_docker volume ls:_** Lista todos os volumes.
- **_docker volume inspect <volume>:_** Exibe informações detalhadas sobre um volume.
- **_docker volume rm <volume>:_** Remove um volume.

### 5. Redes

- **_docker network create <nome>:_** Cria uma nova rede.
- **_docker network ls:_** Lista todas as redes.
- **_docker network inspect <rede>:_** Exibe informações detalhadas sobre uma rede.
- **_docker network connect <rede> <container>:_** Conecta um container a uma rede.
- **_docker network disconnect <rede> <container>:_** Desconecta um container de uma rede.
- **_docker network rm <rede>:_** Remove uma rede.

### 6. Docker Compose

- **_docker-compose up:_** Inicia todos os serviços definidos em um arquivo docker-compose.yml.
- **_docker-compose down:_** Para e remove todos os containers e redes criados pelo docker-compose up.
- **_docker-compose build:_** Constrói ou reconstrói os serviços definidos no docker-compose.yml.
- **_docker-compose ps:_** Lista todos os containers gerenciados pelo docker-compose.
- **_docker-compose logs:_** Exibe os logs dos serviços gerenciados pelo docker-compose.

### 7. Docker Swarm (Orquestração de Containers)

- **_docker swarm init:_** Inicializa um swarm (cluster Docker).
- **_docker swarm join:_** Permite que um nó (máquina) participe de um swarm existente.
- **_docker swarm leave:_** Remove o nó atual do swarm.
- **_docker node ls:_** Lista todos os nós no swarm.
- **_docker service create <opções> <imagem>:_** Cria um novo serviço em um swarm.
- **_docker service ls:_** Lista todos os serviços no swarm.
- **_docker service rm <serviço>:_** Remove um serviço do swarm.

### 8. Outros Comandos Úteis

- **_docker inspect <container/volume/imagem>:_** Exibe informações detalhadas sobre um container, volume ou imagem.
- **_docker diff <container>:_** Exibe as mudanças feitas no sistema de arquivos do container.
- **_docker stats:_** Mostra o uso de recursos em tempo real de todos os containers em execução.
- **_docker top <container>:_** Exibe os processos ativos dentro de um container.
- **_docker cp <container>:<caminho_no_container> <caminho_local>:_** Copia arquivos de dentro do container para o host local.

### 9. Limpeza e Manutenção

- **_docker system df:_** Mostra o uso de espaço em disco pelo Docker.
- **_docker system prune:_** Remove todos os containers, redes, imagens e volumes não utilizados.
- **_docker container prune:_** Remove todos os containers parados.
- **_docker image prune:_** Remove todas as imagens não usadas.
- **_docker volume prune:_** Remove todos os volumes não utilizados.
- **_docker network prune:_** Remove todas as redes não utilizadas.
