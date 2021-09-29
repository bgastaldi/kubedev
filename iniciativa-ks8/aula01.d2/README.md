# KubeDev
## Desafio - 2

- Criar um projeto base como referencia pra uso pela equipe. Como o .NET Core é uma tecnologia que é baseada em JIT, a construção da imagem utiliza o Multistage Build. Então agora você deve usar o projeto de conversão de peso, que está no GitHub do KubeDev e executar ele em container para sua equipe entender por onde começar. Segue o link do projeto no GitHub: https://github.com/KubeDev/conversao-peso Faça um fork do repositório, monte o processo de execução no Docker e compartilha aqui o seu repositório. Essa documentação vai te ajudar https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/docker/building-net-docker-images?view=aspnetcore-5.0 *
- Enumerar as boas práticas que todos devem seguir pra construir as imagens.

## Setup

Lista de imagens no DockerHub.
- bgastaldi/conversao-peso:latest

## Comandos utilizados

Criando a imagem conversão de peso:
``` bash
$ docker build -t bgastaldi/conversao-peso:latest .
```

Executando a Imagem da Aplicação NodeJs:
``` bash
 $ docker run --rm -d -p 8080:80  --name conversao-peso bgastaldi/conversao-peso:latest
```

Subindo a imagem para o Dockerhub:
``` bash
 $ docker push bgastaldi/conversao-peso:latest
```

## Testando
```
http://localhost:8080
```

