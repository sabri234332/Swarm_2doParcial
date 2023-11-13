## Instrucciones para la Implementación del Sistema - TP4
## Este conjunto de instrucciones te guiará a través de la implementación del sistema utilizando Docker Swarm.

## SWARM CON SERVICIOS SOAP Y REST

## PASO 1 Crear las imagenes: Antes de desplegar el sistema, necesitamos construir las imagenes para cada servicio.

## Imagen del servicio REST:
`docker build . -t restapi`
## Imagen del servicio SOAP:
`docker build . -t soapapi`
## Imagen del client
`docker build . -t client`
## Imagen de MySQL:
`docker build . -t mysql-image`

## PASO 2 Desplegar los servicios con swarm

`docker swarm init`

`docker stack deploy -c docker-compose.yml mis-servicios`

## Aclaraciones

Servidor SOAP creado en el puerto 4000

El servidor web se encuentra alojado en localhost:8080