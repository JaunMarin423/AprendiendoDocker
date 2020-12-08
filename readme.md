# En este repo se vera el proceso de aprender docker.


En este repo podremos encontrar mi proceso mediante ente estudio docker y algunos comando útiles este repo más que todo es para llevar un seguimiento en mis repositorios.

## Virtualización

![Scheme](img/docker-vs-virtual-machines.png)

## Como funciona

![Scheme](img/DockerEngine.png)

## Comandos

![Scheme](img/imagencoman.jpg)
![Scheme](img/comandos.jpg)
![Scheme](img/comandos2.jpg)
![Scheme](img/comandos3.jpg)
![Scheme](img/comandos4.jpg)
![Scheme](img/comandos5.jpg)
![Scheme](img/comandos6.jpg)
![Scheme](img/comandos7.jpg)
![Scheme](img/comandos8.jpg)

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
$ docker run ubuntu (corre un ubuntu pero lo deja apagado)
$ docker ps -a (lista todos los contenedores)
$ docker -it ubuntu (lo corre y entro al shell de ubuntu)
-i: interactivo
-t: abre la consola

$ docker stop "name"

$ docker run -d --name proxy nginx (corro un nginx)
$ docker stop proxy (apaga el contenedor)
$ docker rm proxy (borro el contenedor)
$ docker rm -f <contenedor> (lo para y lo borra)
$ docker run -d --name proxy -p 8080:80 nginx (corro un nginx y expongo el puerto 80 del contenedor en el puerto 8080 de mi máquina)
localhost:8080 (desde mi navegador compruebo que funcione)
$ docker logs proxy (veo los logs)
$ docker logs -f proxy (hago un follow del log)
$ docker logs --tail 10 -f proxy (veo y sigo solo las 10 últimas entradas del log)

$ mkdir dockerdata (creo un directorio en mi máquina)
$ docker run -d --name db mongo
$ docker ps (veo los contenedores activos)
$ docker exec -it db bash (entro al bash del contenedor)
$ mongo (me conecto a la BBDD)

shows dbs (listo las BBDD)
use platzi ( creo la BBDD platzi)
db.users.insert({“nombre”:“guido”}) (inserto un nuevo dato)
db.users.find() (veo el dato que cargué)
$ docker run -d --name db -v <path de mi maquina>:<path dentro del contenedor(/data/db mongo)> (corro un contenedor de mongo y creo un bind mount)

Cuando cambie algo este disponible.



```