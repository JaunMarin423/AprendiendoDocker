# En este repo se vera el proceso de aprender docker.


En este repo podremos encontrar mi proceso mediante ente estudio docker y algunos comando útiles este repo más que todo es para llevar un seguimiento en mis repositorios.

## Virtualización

![Scheme](img/docker-vs-virtual-machines.png)

## Como funciona

![Scheme](img/DockerEngine.png)

## Comandos

![Scheme](img/imagencoman.jpg)

```docker
$ docker run hello-world (corro el contenedor hello-world)
$ docker ps (muestra los contenedores activos)
$ docker ps -a (muestra todos los contenedores)
$ docker inspect <containe ID> (muestra el detalle completo de un contenedor)
$ docker inspect <name> (igual que el anterior pero invocado con el nombre)
$ docker run –-name hello-platzi hello-world (le asigno un nombre custom “hello-platzi”)
$ docker rename hello-platzi hola-platzy (cambio el nombre de hello-platzi a hola-platzi)
$ docker rm <ID o nombre> (borro un contenedor)
$ docker container prune (borro todos lo contenedores que esten parados)

```