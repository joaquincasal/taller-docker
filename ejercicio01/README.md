# Ejercicio 1: Contenedor nginx

Comando: `docker run -v $(pwd):/usr/share/nginx/html:ro -p 8080:80 nginx`  
Usamos -v para montar un volumen con los archivos html a servir en el directorio default de nginx.  
Usamos -p para exponer el puerto y poder acceder desde un navegador desde el host.  
Una vez que el contenedor está corriendo, podemos acceder al archivo index.html mediante un navegador en localhost:8080 o localhost:8080/index.html. Para el otro archivo, lo accedemos en localhost:8080/otro.html
