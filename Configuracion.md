## Actualización del Sistema
Primero, es necesario ejecutar los siguientes comando:
- sudo apt update
- sudo apt upgrade

Con ellos mantendremos nunestro equipo totalmente actualizado para descargar las últimas versiones de los softwares necesarios

## Instalación de paquetes
Una vez instaladas las actualizaciones, instalaremos el paquete isc-dhcp-server:
- sudo apt install isc-dhcp-server

## Desactivar NetworkManager
Antes de empezar a configurar la red, desactivaremos NetworkManager con los siguientes comandos:
- systemctl disable NetworkManager
- systemctl stop NetworkManager

El primer comando hará que no se active cuando se inicie el sistema, y el segundo lo apagará en ese mismo momento

## Configurar Red
1. Pondremos como tarjeta de red principal del equipo un "adaptador puente", y una segunda tarjeta como "red interna".
2. Una vez instaladas las tarjetas de red, se empezará a configurar el fichero /etc/network/interfaces en ambos equipos.
