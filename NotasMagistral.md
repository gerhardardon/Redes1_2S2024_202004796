# Notas de clase magistral redes de computadoras 1
---
10/08/2024
## Capas de modelo OSI y TCP-IP
- Network acces: del modelo tcp-ip se pueden encontrar los medios de conexion alambricos e inalambricos.
- Internet: todos los protocolos para el acceso a internet.
- Host-to-Host: se conectara mediante modelos tcp y udp hacia otros hosts.
- Process/Application: son los protocolos que utilizan las aplicaciones, el mas común es telnet, tambien hay protocolos para comunicaciones, enviar archivos, imagenes, etc.
### TCP Segment Format 
netstat -pan tcp
netstat = estadisticas de red
-p = protocolo
-a = activas 
-n = network  
Este comando nos dara las conexiones establecidas por el modelo tcp y regresa el siguiuente formato:
IP_LOCAL : PUERTO_LOCAL(pto. aleatorio) - IP_REMOTO : PUERTO_REMOTO(pto. conocido)

Para realizar troubleshooting se deben validar que los pasos del three-way-handshake se cumplan correctamente
