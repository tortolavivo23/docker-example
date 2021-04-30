# AIS  Heroku

Este proyecto consta de un servidor REST sencillo para la gestión de items.

## Construir la aplicación (en local)

Para construir el JAR del proyecto (y lanzar los test):

```
    ./mvnw clean package
```

## Lanzar la aplicación en local (en local)

Para lanzar la aplicación el local:

```
    java -jar target/items-0.0.1-SNAPSHOT.jar 
```

## Construimos y subimos la imagen a DockerHub

```
    docker login
    docker build -t <my_user>/items:v1 .
    docker push <my_user>/items:v1
```

## Lanzamos la imagen CAMBIO

```
    docker run -p 8080:8080 <my_user>/items:v1
```

