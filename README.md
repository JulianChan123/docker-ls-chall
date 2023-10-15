# docker-ls-chall

## Documentación del ejercicio - EQUIPO 2
Integrantes del equipo

 - Victor Chan
 - Julian Chan
 - Luis Ku

Documentación del reto de realizar 2 imágenes de Docker y realizar el docker-compose

Cuando se descargue el proyecto lanzamos el comando para compilar y levantar el proyecto:

```shell
   docker build -t nombre_de_la_imagen .
```

Después de ejecutar el comando anterior para construir la imagen, ahora tenemos que correr la imagen con el siguiente comando

para utilizar la aplicación de **weatherApp** utilizamos el puerto **5173**

```shell
   docker run -d -p 5173:80 nombre_de_la_imagen
```

Una vez corriendo el contenedor podemos revisar que esté arriba con el comando:

```shell
   docker ps
```

Si ahora queremos detener la aplicación, después de ubicarla con el comando "ps", seleccionamos el ID del servicio y lo colocamos con:
```shell
   docker stop id_container
```

## Docker compose comandos utilizados

Cuando queremos compilar el proyecto con docker compose y el archivo no tiene algun nombre especifico utilizamos:

```shell
   docker-compose build
```

Una vez compilado el proyecto, para levantarlo utilizamos:

```shell
   docker-compose up