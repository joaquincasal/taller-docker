# Ejercicio 7: JobVacancy docker-compose

Q: ¿Cuántos contenedores se están ejecutando?  
A: Dos contenedores, uno para la app web y otro para la base de datos.

Q: ¿Cuales son las imágenes en las que están basados los mencionados contenedores?  
A: El contenedor web está basado en nicopaez/jobvacancy-ruby:1.3.0 y la db en postgres:14.4-alpine

Q: ¿Puedes leer el docker-compose.yml y describir lo que hace cada una de sus lineas?  
A: El container db define la imagen base a utilizar (versión alpine de postgres) y define una variable de ambiente para la contraseña de la base de datos. El container web define la imagen base a utilizar, mapea los puertos 3000 del host y del container, setea variables de ambiente y permite comunicar al container con el container db mediante 'link'. También utiliza depends_on para indicar que el contenedor de la base de datos debe levantar primero que el web.

Q: Dado que cada contenedor corre en forma aislada ¿Cómo es posible que esos contenedores se vean entre sí?  
A: Pueden comunicarse porque se está utilizando link.