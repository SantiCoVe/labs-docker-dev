# Documentacion primer laboratorio

## Imagen oficial de ubuntu
Using default tag: latest
latest: Pulling from library/ubuntu
9c704ecd0c69: Pull complete 
Digest: sha256:2e863c44b718727c860746568e1d54afd13b2fa71b160f5cd9058fc436217b30
Status: Downloaded newer image for ubuntu:latest
docker.io/library/ubuntu:latest

## Imagen de python version especifica
3.9: Pulling from library/python
ca4e5d672725: Pull complete 
30b93c12a9c9: Pull complete 
10d643a5fa82: Pull complete 
d6dc1019d793: Pull complete 
c387064957b7: Pull complete 
26766ebde481: Pull complete 
8a42d17fd0e2: Pull complete 
79eda865cc8a: Pull complete 
Digest: sha256:fea84f3a3b72c41efe7fc3b07ae209c6856b852b942c05fa88b747b74f70e711
Status: Downloaded newer image for python:3.9
docker.io/library/python:3.9

## Ejecutamos docker en el puerto 8800:80
a21e027d762933f74afcc2cd19308dd559841e6530ef5ed4cddb5793f3edf63b

## Ejecucion de ubuntu en modo iterativo
root@49a2556e6b41:/#

## Pull de apache con docker
Using default tag: latest
latest: Pulling from library/httpd
efc2b5ad9eec: Already exists 
fce1785eb819: Pull complete 
4f4fb700ef54: Pull complete 
f214daa0692f: Pull complete 
05383fd8b2b3: Pull complete 
88ad12232aa1: Pull complete 
Digest: sha256:932ac36fabe1d2103ed3edbe66224ed2afe0041b317bcdb6f5d9be63594f0030
Status: Downloaded newer image for httpd:latest
docker.io/library/httpd:latest

## Ejecucion en segundo plano de apache
dc9dba7d33081706d9728a30a2931be2802d4883a98ae4811fcd250b300927e4

## Visualizamos todos los contenedores
CONTAINER ID   IMAGE     COMMAND                  CREATED          STATUS                       PORTS                                   NAMES
dc9dba7d3308   httpd     "httpd-foreground"       2 minutes ago    Up 2 minutes                 0.0.0.0:8000->80/tcp, :::8000->80/tcp   youthful_bhaskara
49a2556e6b41   ubuntu    "bash"                   15 minutes ago   Exited (130) 7 minutes ago                                           youthful_ramanujan
a21e027d7629   nginx     "/docker-entrypoint.…"   16 minutes ago   Up 16 minutes                0.0.0.0:8080->80/tcp, :::8080->80/tcp   sweet_brattain

## Eliminacion de contenedor ubuntu
49a2556e6b41

## Visualizacion despues de eliminar ubuntu
CONTAINER ID   IMAGE     COMMAND                  CREATED          STATUS          PORTS                                   NAMES
dc9dba7d3308   httpd     "httpd-foreground"       7 minutes ago    Up 7 minutes    0.0.0.0:8000->80/tcp, :::8000->80/tcp   youthful_bhaskara
a21e027d7629   nginx     "/docker-entrypoint.…"   21 minutes ago   Up 21 minutes   0.0.0.0:8080->80/tcp, :::8080->80/tcp   sweet_brattain

## Eliminar todos los contenedores detenidos
Total reclaimed space: 0B