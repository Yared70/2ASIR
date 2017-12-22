# Servidor Web Apache Linux

#### Apache

* Comenzamos instalando Apache y comprobando su funcionamiento

![1](img/1.png)

* Comprobamos /var/www/

![2](img/2.png)

* Accedemos a localhost

![3](img/3.png)

* Añadir línea www.miempresa.com asociada a IP servidor en /etc/hosts

![4](img/4.png)

* Reiniciamos Apache

![5](img/5.png)

#### Php

* Instalar php

![6](img/6.png)

![7](img/7.png)

* Comprobamos acceso

![8](img/8.png)

### Crear hosts virtuales en Apache

* Creamos una carpeta public_html para alojar el index

![9](img/9.png)

* Creamos el virtualhost dentro de Apache2 y creamos el enlace simbolico

![10](img/10.png)

* Añadimos la página al archivo etc/hosts

![11](img/11.png)

* Comprobamos

![12](img/12.png)

#### Sitios web seguros

* Empezamos creando las claves para el sitio web pagos que crearemos mas adelante

![13](img/13.png)

![14](img/14.png)

![15](img/15.png)

* Creamos el virtual host en sites-available

![16](img/16.png)

* Al comprobar vemos que funciona pero al no tener un certificado oficial nos sale esta pantalla

![17](img/17.png)

#### Carpetas privadas

* Empezamos creando la carpeta en /var/www/ con el nombre de la página a crear y creamos el archivo .htaccess dentro de esa carpeta

![18](img/18.png)

* Creamos la password para la carpeta y el usuario

![19](img/19.png)

* Reiniciamos el servicio

![21](img/21.png)

* Creamos el virtualhost

![22](img/22.png)

* Y comprobamos el acceso

![23](img/23.png)

#### Mysql y phpmyadmin

* Empezamos instalando mysql-server

![24](img/24.png)

* Instalamos el modulo php de Mysql

![25](img/25.png)

> Aquí instalabamos phpmyadmin en la carpeta del host empleados, pero al acceder desde el navegador daba error de la extensión mysqli. Tras dos días en los que se intento arreglar editando los archivos de configuración y reinstalando mysql, php y apache desde cero en clase con el profesor, no se pudo solucionar el problema, por lo que, no se pudo seguir con la actividad
