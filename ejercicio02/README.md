# Ejercicio 2: Publica una imagen

Pasos seguidos:

1. Ejecutar `docker image pull nicopaez/pingapp:3.0.0`
1. Ejecutar `docker tag nicopaez/pingapp:3.0.0 joaquincasal/pingapp:1.0.0`
1. Ejecutar `docker login` y seguir los prompts
1. Ejecutar `docker push joaquincasal/pingapp:1.0.0`

Comando para descargar la imagen publicada: `docker image pull joaquincasal/pingapp:1.0.0`
