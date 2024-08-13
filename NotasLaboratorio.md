# Notas del laboratorio redes de computadoras 1
---
27/09/2024
## TCP-IP y Modelo OSI 
--- 
03/08/2024
## Cableado Estructurado 
Es un sistema de cables que permite establecer infraestructura de telecomunicaciones dentro de una compañia. Se deben seguir ciertos estandares. 
**Acometida:** Es un subsistema que engloba cables, hardware de conexion, es unicamente la entrada de un servicio externo
**Cuarto de equipos:** Sirven para distribuir el sistema de telecomunicaciones 
**Cableado vertical:**(backbone o troncal) Permite la conexion entre el cuarto de equipos y los diferentes cuartos, la fibtra optica es el cableado mas adecuado para esto
**Cuarto de comunicaciones:** Distribuye por el cableado horixontal a los distintos pisos
**Cableado horizontal:** Cableado que se extiende al area de tarbajo, generalmente pasa por medio de una cruzada horizontal llamada cross conect
**Area de trabajo:** Area de trabajo

NOTAS: modo multimodo (se puede enviar y recibir al mismo tiempo la info) y unimodo (solo enviar o recibir)

El cabaleado horizontal se compone de rutas y espacios verticales. Se deben de tener ciertas consideraciones como contener la mayor cantidadd e cables individuales 

### Factores a tomar en cuenta 
Atenuacion o ruido
Capacitancia del cable
### Normas y estandares del cableado 
**Norma:** Establecen un lenguaje comun entre empresas y consumidores 
**Estandar:** Es la norma ya aprobada 
Los mas comunes son TIA ANSI EIA ISO IEEE:
**TIA:** Acreditada por ANSI para desarrollar estandares industriales, se utiliza en radios privadas, torres de celulares, terminales, satelites, etc.
**ANSI:** Organizacion privada y sin fines de lucro para identificar y unificar estandares, Esta no desarrolla estandares, mas bien proporciona un marco para estandares justos.
**EIA:** Organizacion comercial de estandares estadounidenses, ahora es gestionado por TIA
**IEEE:** Es una de las organizaciones lideres de estandares en el mundo 

### Medios de Transmision
**Medios de red:** Cable de cobre, fibra optica y medios inalambricos 
**Cable par trenzado:** Tiene dos conductores aislados para anular interferencias en los cables. Existen ditintos tipos de este cable (UTO, FTP, STP...) Tambien categorias de cables (CAT1 - CAT8) las cuales manejan distintas velocidades y frecuencias para aplicaciones fisicas distintas (de CAT4 en adelante es recomendable para el envio de datos)
**Cable de red directo:** Se utiliza para conectar dispositivos diferentes como un ordenador a un switch, mantiene la secuencia de pines para que se comuniquen directamente 
**Cable de red cruzado:** Para dispositivos iguales, ya que los pines estan cruzados para evitar interrupciones y garantizar comunicacion directa y efectiva
**Serial DCE:** Conecta un dispositivo que actua como equipo de comunicaciones de datos
**Serial DTE:** Conecta dispositivos que actuan como terminales de equipos de datos, Por ejemplo ordenadores y switches

NOTA: EJEMPLO PRACTICO PACKET TRACER
Con dispositivos iguales (routers) recomendado, aplicar serial, tambien se puede cable cruzado como 2da opc.

---
10/08/2024
## Capa de Acceso 
Capacidad de interactuar con un sistema ya sea de manera local o remota, Para conectarse de forma remota se puede utilizar ssh, vpn, escritorios remotos y TeamViewer (y herramientas similares)

Dispositivos de capa de acceso:
- hubs: dispositivos mas simples, parecidos a un router, no pueden enviar y recibir al mismo tiempo.
  Si dos o mas dispositivos desean enviar mensaje al mismo tiempo se da una colision (dominio de colision)
- switch: toma decisiones basada en la informacion contenida, puede mandar mensajes a un dispositivo especifico, el switch si puede manejar direcciones mac.
  Tabla de direcciones mac, el switch valida sib la direccion mac a la que se quiere enviar el mensaje forma parte del switch.
  El dominio de colision se da generalmente en topologias de estrella, o cuando tenemos muchos hosts conectados.
- brodcast: va de uno a todos, indica que dsipositivo lo envia y cuales son los que lo recibe, el dominio de brodcast se puede ver como un dominio de difusion. 
### ARP 
Protocolo para descubrir y almacenar direccoines mac dentro de un host de la red, esta sigue una serie de pasos:
solicitud arp -> respuesta arp -> informacion actualizada arp
### Access Point
Tiene la capacidad de conectar host a una red local de manera inalambrica, tenemos distintos tipos de access point.
- De raiz: se conecta directamente a una LAN para poder conectar inalambricamente
- Repetidor: cambia el alcance de la infraestructura que ya poseemos. 
- Puentes: se pued eusar para unir varias redes
- Unidad central en red totalmente inalambrica: es un concentrador para conectar host a un punto central de comunicaciones y aumentar la cantidad de usuarios inalambricos
### Firewall
Sistema de seguridad que restringe el ttrafico a una red privada, protege los paquetes de datos de una forma selectiva.

NOTA: LECTURA DE PRACTICA #1 