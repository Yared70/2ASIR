# Instalación de un servidor DHCP en Windows

#### Crear un manual de instalación y configuración de un servidor DHCP en una máquina con Windows Server.

*Empezamos instalando el DHCP en el windows server. Para esto nos vamos a activar roles y caracteristicas y buscamos el DHCP*

![imagen](img/1insroldhcp.png)

![imagen](img/2insdhcp.png)

![imagen](img/3configurardhcp.png)

![imagen](img/4confdhcp.png)

*Ahora, una vez instalado el DHCP vamos a crear un ámbito. Para esto en el panel del servidor, nos vamos a herramientas y a DHCP.*

*Una vez aqui, nos vamos a crear ámbito como se ve en la imagen*

![imagen](img/5crearambito.png)

*El ámbito lo configuramos dependiendo de la ip que tengamos en el servidor y los rangos que queramos asignar*

![imagen](img/6ambito.png)

![imagen](img/7ambito.png)

![imagen](img/8amb2.png)

![imagen](img/9amb.png)

![imagen](img/10amb.png)

![imagen](img/11amb.png)

*Ahora crearemos un segundo ámbito*

> El segundo ámbito lo crearemos en la misma red, pero se puede crear en otra si se posee mas de una tarjeta de red instalada

![imagen](img/13amb2.png)

![imagen](img/14amb2.png)

![imagen](img/14_2amb2.png)

![imagen](img/15amb2.png)

*Ahora que tenemos los dos ámbitos creados, los todos en un superámbito*

![imagen](img/16supamb.png)

![imagen](img/17superamb.png)

![imagen](img/18superamb.png)

![imagen](img/19superamb.png)

*Una vez creado el superámbito, nos vamos al ámbito 1 para crear una reserva por MAC del cliente*

![imagen](img/23reserv.png)

*Ahora nos vamos al cliente y comprobamos si funciona*

![imagen](img/12amb.png)

>Aquí vemos que el cliente tiene por dhcp la ip que le asignamos en la reserva

*Ahora como prueba final, nos vamos al servidor y desactivamos el superámbito. Al hacerlo comprobaremos como el cliente no obtiene ninguna dirección por dhcp*

![imagen](img/20descamb.png)

![imagen](img/21finalcon.png)

>Aquí vemos como se nos da la dirección 169.254.114.53 que es una predefinida que nos da el dhcp si no puede obtener una correcta. Esto se ve en que no tenemos una puerta de enlace predeterminada
