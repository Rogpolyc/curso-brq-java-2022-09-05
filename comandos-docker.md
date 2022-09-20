# Principais comandos

## Como iniciar um container (que ainda não existe)?

```
    docker run NOME-DA IMAGEM

    EX: docker run docker/getting-started
```

## para listar os container que estão em execução

```
    docker ps
```

# Se eu quiser parar a execuçõ de um container:

```
    docker stop NOMEDOCONTAINER
    Ex: docker stop elated_poitras
```

# Se eu quiser iniciar um container que já existe:

```
    docker start NOMEDOCONTAINER
    Ex: docker start elated_poitras
```

# Para remover um container:

Obs: o container deve estar parado!!!!!

```
    docker run NOMEDOCONTAINER
    Ex: docker rm elated_poitras
```

# Eu posso estipular o nome de um container

Obs: exemplo na criação do container
O nome da imagem sempre precisa ser o último parâmetro do docker run

```
    docker run  --nane NOMEDOCONTAINERDESEJO NOMEDAIMAGEM
    Ex: docker run --name hello-world docker/getting-started
```

# redirecionar a requisição da máquina hospedeira para um container docker

Obs: exemplo na criação do container


```
    docker run  --name NOMEDOCONTAINERDESEJO -p PORTA-HOSPEDEIRO:PORTA-CONTAINER  NOMEDAIMAGEM
    Ex: docker run --name hello-world -p 80:80  docker/getting-started
```