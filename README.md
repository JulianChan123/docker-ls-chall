# docker-ls-chall

## Documentación del ejercicio - EQUIPO 2
Integrantes del equipo

 - Victor Chan
 - Julian Chan
 - Luis Ku ( no ayudo )

Documentación del reto de realizar 2 imágenes de Docker y realizar el docker-compose

Para poder correr el docker es necesario poner docker-compose up -d
donde -d se usa para que docker funcione en segundo plano

```shell
   docker-compose up -d
```
para poder cambiarnos de aplicacion se tiene que cambiar de puerto de la siguiente forma
**localhost: [puerto de proyecto definido]**

para utilizar la aplicación de **weatherApp** utilizamos el puerto **5173**

```shell
   localhost:5173
```
para utilizar la aplicación de **TodoList-simple** utilizamos el puerto **3000**

```shell
    localhost:3000
```

para detener el funcionamiento del docker colocamos el siguiente comando:
```shell
   docker-compose down