# Ejercicio 13: JobVacancy en k8s

- Edité el archivo recibido web-deployments.yaml para agregar un container de postgres al mismo pod de la webapp.
- Creé un configmap para las variables de ambiente de la webapp
- Creé un secret con credenciales de la base datos. Es compartido por ambos containers (no me pareció que valiera la pena separarlo).
- Agregué un service para poder acceder desde una url pública a la webapp.

Url: https://jobvacancy-joaquincasal.cloud.okteto.net/