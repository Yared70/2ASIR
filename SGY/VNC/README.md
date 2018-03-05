# Conexiones remotas con VNC

## Instalación en Windows
___

*Empezamos con la instalación de TightVNC en el servidor Windows*

![imagen](img/1vncserver.png)

>Como se ve en la imagen, en el servidor solo se instala el server

*Ahora lo instalamos en el cliente, esta vez solo el viewer al ser el cliente*

![imagen](img/2vnccliente.png)

*Una vez instalado en los dos solo falta hacer la prueba de conexión desde el cliente al servidor*

![imagen](img/3con.png)

![imagen](img/4finalwin.png)

## Instalación en OpenSUSE
___

*Empezamos configurando en el servidor el VNC desde Yast. En este caso ya viene instalado por defecto*

![imagen](img/1osvnc.png)

 *En este caso, como en windows, le damos al servidor la capacidad de ejercer cambios en el cliente*

![imagen](img/2osvnc2.png)

![imagen](img/3osvnc3.png)

*Ahora en el cliente hacemos lo mismo, salvo cambiando el primer paso*

![imagen](img/4osvncc.png)

___

*Una vez instalado tanto en el cliente como en el servidor, probamos la conexión*

![imagen](img/6vncconect.png)

> En este caso hay que añadir :5901 ya que en este caso es el puerto destinado a VNC

*Al darle a conectar veremos como controlamos el otro pc*

![imagen](img/7vncserv.png)

>Cree el archivo "aqui estuvo el server" como prueba de la conexión. Aquí se ve como si cerramos la sesion y vamos al cliente, el archivo está en el escritorio

![imagen](img/8cliente.png)

*Ahora lo haremos a la inversa, desde el cliente nos conectamos al server*

![imagen](img/10clienteaser.png)

![imagen](img/11vnccli.png)

>Hacemos la misma prueba para ver si funcionó y vemos que si

___

#### Conexión entre distintos SO

*Para terminar comprobaremos la conexión desde OpenSUSE a Windows*

![imagen](img/conect.png)

![imagen](img/conect2.png)

>Vemos como se ve en las dos pantallas y además se puso en negro el escritorio
