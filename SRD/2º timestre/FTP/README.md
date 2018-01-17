# Servidor FTP en Windows Server 2012

Empezamos instalando el servicio FTP desde el IIS

![1](img/1.png)

#### Primer sitio

Accedemos al IIS y creamos el sitio ftp: `ftp.miempresa.com`. Este ftp tendra acceso a todo el directorio C:/ pero solo el Administrador.

![2](img/2.png)

![3](img/3.png)

![4](img/4.png)

![11](img/11.png)

Comprobamos el acceso al ftp desde el navegador

![5](img/5.png)

Y comprobamos desde el explorador de archivos

![6](img/6.png)

Y por ultimo comprobamos desde el cliente

![7](img/7.png)

Ahora instalamos el winscp desde el cliente

![8](img/8.png)

![9](img/9.png)

![10](img/10.png)

Y comprobamos el funcionamiento

![12](img/12.png)

#### Segundo Sitio

El segundo sitio está enlazado a la carpeta wwwroot de inetpub. Permitimos acceso a todos, sin usuarios anonimos y con la posibilidad de usar ssl

![13](img/13.png)

![14](img/14.png)

![15](img/15.png)

Comprobamos el acceso

![18](img/18.png)

Y comprobamos desde el cliente

![16](img/16.png)

![17](img/17.png)

#### Tercer Sitio

Lo enlazamos a una carpeta elegida por nosotros, permitimos acceso anónimo y solo se puede consultar y leer

![19](img/19.png)

![21](img/21.png)

![22](img/22.png)

Y comprobamos:

![25](img/25.png)

#### Comprobaciones restantes

Todos los sitios activos:

![26](img/26.png)

![27](img/27.png)

![28](img/28.png)

Administrador de DNS:

![23](img/23.png)

Solución a la pregunta: **Encontrar una solución para que nuestro servidor ofrezca varios sitios FTP simultáneamente**

*Esto lo solucionamos asignando un puerto distinto a cada FTP.*

# Servidor FTP en Linux

Comenzamos instalando el ssh por la terminal con `apt-get install ssh`

![29](img/29.png)

Creamos dos usuarios (usuario1 y usuario2) con distintos permisos, administrador y usuario normal respectivamente

![30](img/30.png)

Comprobamos el acceso desde un cliente y ejectuamos un programa gráfico en este caso gedit.

![31](img/31.png)

Ahora probamos el acceso por sftp y realizamos operaciones, en este caso una descarga con get

![33](img/33.png)

Tras esto comprobamos a subir un archivo desde el cliente al servidor por scp. Dependiendo de los permisos del usuario nos dejara o no dependiendo de la carpeta de destino

![34](img/34.png)

![35](img/35.png)

Por ultimo instalamos proftpd y comprobamos su uso

![36](img/36.png)

![37](img/38.png)
