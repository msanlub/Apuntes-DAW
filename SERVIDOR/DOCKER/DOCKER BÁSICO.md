### DESCRIPCIÓN

Es un "emulador" de entornos aislado para poder ejecutar programas sin que afecte a mi sistema operativo (SO) y pudiendose llevar y replicar en otros SS.OO. o entornos.

Docker consta de imágenes y contenedores:

1. Una **imagen** es la especificación inerte, inmmutable, una foto del estado y de unas piezas de software que incluyen desde la aplicación que queremos ejecutar hasta las librerias y todo lo necesario para que corra encima del sistema operativo en el cual se ejecuta.
2. Un **contenedor** es un entorno aislado con la instanciación de una imagen, el cual se puede configurar.

### PRINCIPALES COMANDOS

Listado de imágenes de docker instaladas:

```shell
  docker images
```

Listado de contenedores de docker creados:

```shell
  docker container ls
```

o su alias

```shell
  docker ps
```

Para bajar una de imágen de docker del [docker hub](https://hub.docker.com/):

```shell
  docker pull IMAGEN
```


### MÁS COMANDOS

```shell
  docker build -t NOMBRE_IMAGEN .
  docker run NOMBRE_IMAGEN
  docker inspect CONTENEDOR-ID
  docker logs CONTENEDOR-ID
  docker exec -it CONTENEDOR /bin/bash
  docker start / stop / restart CONTENEDOR-ID
  docker stop CONTENEDOR-ID
  docker rm CONTENEDOR-ID
  docker rmi IMAGEN
  docker start nombre_contenedor
```

- **build** se utiliza para generar/contruir una imagen a partir del Dockerfile
- **run** se utiliza para lanzar el contenedor a partir de una imagen
- **inspect** se utiliza para obtener información a bajo nivel del contenedor
- **logs** se utiliza para ver la salida generada por consola al ejecutar el contenedor
- **exec** se utiliza para ejecutar comandos en un contenedor que está ejecutandose
- **stop** se utiliza para parar la ejecución de un contenedor que está ejecutandose
- **rm** se utiliza para borrar un contenedor
- **rmi** para borrar una imagen creada
- start para correr un contenedor en pausa ya creado
