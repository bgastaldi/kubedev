# KubeDev
## Desafio - 1

- Faça um fork do repositório (https://github.com/KubeDev/conversao-temperatura), monte o processo de execução no Docker e compartilha aqui o seu repositório.
- Enumerar as boas práticas que todos devem seguir pra construir as imagens.

## Setup

Lista de imagens no DockerHub.
- bgastaldi/conversao-temperatura:latest

## Comandos utilizados

Criando a imagem conversão de temperatura:
``` bash
$ docker build -t bgastaldi/conversao-temperatura:latest .
```

Executando a Imagem da Aplicação NodeJs:
``` bash
 $ docker run --rm -d -p 8080:8080  --name conversao-temperatura bgastaldi/conversao-temperatura:latest
```

Subindo a imagem para o Dockerhub:
``` bash
 $ docker push bgastaldi/conversao-temperatura:latest
```

## Testando
```
http://localhost:8080
```

