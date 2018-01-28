# Instalación servicio SMTP en Windows 2012 Server

Instalamos el servivio SMTP desde el IIS

![](img/1.png)

![](img/2.png)

Ahora entrando al IIS 6.0 configuramos el SMTP como se pide en la actividad

![](img/3.png)

![](img/4.png)

![](img/5.png)

![](img/6.png)

![](img/7.png)

![](img/8.png)

Ahora creamos un nuevo dominio desde el IIS 6.0

![](img/9.png)

![](img/10.png)

![](img/11.png)

Y comprobamos desde el cliente si hace ping al dominio

![](img/13.png)

Ahora instalamos un cliente de correo en la máquina cliente. En este caso usamos opera mail.

![](img/14.png)

Tras instalarlo, creamos y configuramos una cuenta de correo

![](img/15.png)

![](img/16.png)

![](img/17.png)

![](img/18.png)

Aqui configuramos el servidor donde instalamos el SMTP

![](img/19.png)

Por ultimo comprobamos si funciona mandando un correo a una cuenta gmail real, y vemos como llega el correo

![](img/20.png)

Tras esto probamos añadiendo el cifrado tls y con otro dominio

![](img/21.png)

# Configuración de hMailServer en Windows Server 2012

Empezamos desinstalando el servicio SMTP para evitar conflictos e instalamos el hMailServer

![](img/22.png)

![](img/23.png)

![](img/24.png)

Creamos los dos dominios nuevos dns que se piden en la actividad

![](img/25.png)

![](img/27.png)

Y los añadimos en el hMailServer

![](img/28.png)

Ahora ejecutamos los diagnosticos y solucionamos los fallos que nos indiquen

![](img/29.png)

![](img/30.png)

Ahora creamos dos usuarios en cada dominio

![](img/31.png)

Creamos dos entradas en el dns

![](img/32.png)

Y configuramos las cuentas con diferentes opciones

![](img/33.png)

![](img/34.png)

![](img/35.png)

Ahora configuramos las propiedades de las cuentas para el correo

![](img/36.png)

![](img/37.png)

Y por ultimo comprobamos el funcionamiento mandando correos entre las cuentas

![](img/38.png)

![](img/39.png)

Y lo mismo pero creando una lista de distribución

![](img/40.png)

![](img/41.png)
