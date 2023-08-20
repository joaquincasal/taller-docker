# Ejercicio 10: CMD vs ENTRYPOINT

ENTRYPOINT define el ejecutable que correrá cuando corramos un contenedor con la imagen, por defecto es `/bin/sh -c`. Entonces si yo ejecuto `docker run -it IMAGEN bash` lo que se termina ejecutando es `/bin/sh -c bash`.  
CMD define parámetros que se pasan al ENTRYPOINT. En el comando anterior, `bash` cumple el rol de CMD. Sería equivalente indicar en el Dockerfile `CMD ["bash"]`