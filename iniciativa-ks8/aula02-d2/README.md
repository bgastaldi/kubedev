# KubeDev
## Desafio - 2

- Implementar o Kubernetes com o Conversão de Peso.

## Setup

Lista de imagens no DockerHub.
- bgastaldi/conversao-peso:latest

## Comandos utilizados

Criando o cluster:
``` bash
$ kind create cluster --config=cluster.yaml --name=kubedev
$ kubectl cluster-info --context kind-kubedev
```

Aplicando os manifestos de configurações:
``` bash
 $ kubectl apply -f cluster.yaml
 $ kubectl apply -f deployment.yaml
```

Verificando os pods:
``` bash
 $ kubectl get pods
```

Verificando todos os serviços:
``` bash
 $ kubectl get all
```

## Testando
```
http://localhost:8080
```

