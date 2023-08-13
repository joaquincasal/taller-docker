# Ejercicio 8: Creación de cluster balanceado

Para correr los dos containers de la aplicación y el load balancer correr `docker compose up`.  
Mediante el comando `replicas` indicamos que queremos dos instancias del contenedor web.  
Por otro lado, la configuración de nginx indica pasar las requests recibidas a dichos contenedores.