# Ejercicio 11: Telegram Bot

Una vez seteada la configuración para usar Okteto ejecuté `kubectl apply -f ejercicio11/pod.yml` parado en la raíz de mi repositorio. Verifiqué que estuviera corriendo con `kubectl get pods` (y enviando el comando /version al bot). Luego borré el pod con el mando `kubectl delete pod telegram-bot`.