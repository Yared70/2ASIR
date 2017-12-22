# Iptables 2

### 1. Describe cómo utilizar hping para verificar si el servicio FTP está activado y si se encuentra redireccionado en un host interno.

Hping3 es una aplicación de terminal para Linux que nos va a permitir analizar y ensamblar fácilmente paquetes TCP/IP. A diferencia de un Ping convencional que se utiliza para enviar paquetes ICMP, esta aplicación permite el envío de paquetes TCP, UDP y RAW-IP.

Para verificar si el servicio FTP está activado necesitamos utilizar el siguiente comando y si se encuentra redireccionado en un host interno.

> Hping3 -S hostinterno -p puertoftp

**hostinterno** → la ip del host al que queremos verificar el servicio ftp

**puertoftp** → puerto para verificar el servicio en este caso el puerto 21


### 2.Construye una orden de iptables que acepte el tráfico TCP cuyo puerto de destino sea el 80 en el interfaz eth1 con IP origen 10.10.10.10.

Para aceptar el tráfico TCP cuyo puerto de destino sea el puerto 80 en la interfaz eth1 y con la IP origen 10.10.10.10:

> iptables -A INPUT -i eth1 -d 10.10.10.10 -m state --state NEW -p tcp --dport 80 -j ACCEPT

### 3.Construir una regla con iptables que cierre todos los puertos desde el 1 al 1024.

Para cerrar un rango de puertos desde el 1 al 1024 necesitamos crear la siguiente regla:

> iptables -I INPUT -p TCP --dport 1:1024 -j DROP


### 4.Describe qué parámetros hay que modificar para que un equipo no responda a un ping externo.

Para que un equipo no responda a un ping externo necesitamos crear una iptable:

> iptables -A INPUT -p ICMP -j DROP

Con esto le diremos que todo el tráfico recibido de ICMP (que es el protocolo de la herramienta ping) lo rechace automáticamente.
