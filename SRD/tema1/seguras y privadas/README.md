# Carpetas seguras y privadas

#### Carpetas seguras
----
* Crea una nueva zona de búsqueda directa en los servicios DNS asociado al dominio miEmpresa. Crea
también una carpeta miEmpresa en C:\ y una subcarpeta ‘principal’

![1](img/seguras/1.png)

![2](img/seguras/2.png)

* Crea un nuevo sitio web denominado miEmpresa en IIS asociado a la subcarpeta anterior y con
acceso a través de la dirección "www.miEmpresa.com"

![3](img/seguras/4.png)

* Crea un nuevo
sitio web (denominado ‘pagos’) como subdominio de miEmpresa (pagos.miEmpresa.com) y configura
este último para ser accedido de forma segura, vía ‘https’

![4](img/seguras/5.png)

![5](img/seguras/6.png)

![6](img/seguras/8.png)

* Configura el nuevo sitio para
que se pueda acceder (sólo) como sitio web seguro (https) con un Certificado Autofirmado

![7](img/seguras/9.png)

![7](img/seguras/10.png)

![7](img/seguras/11.png)

* Crearemos un nuevo sitio seguro (tienda.miempresa.com) con la generación de
un Certificado Digital a través de la aplicación OpenSSL.

![8](img/seguras/13.png)

![8](img/seguras/15.png)

![8](img/seguras/16.png)

* A través de OpenSSl genera un nuevo certificado de servidor: generar una clave privada
de la entidad certificadora, crear un certificado digital de la entidad certificadora y, finalmente,
crear un certificado digital de nuestra web.

![9](img/seguras/17.png)

![9](img/seguras/18.png)

![9](img/seguras/19.png)

* Importar el nuevo certificado de servidor creado para completar la petición pendiente en
nuestro sitio seguro ‘pagos’.

![9](img/seguras/20.png)

* Requerir que nuestros sitio seguros sólo se pueda acceder mediante una conexión segura

![10](img/seguras/21.png)

*  Acceder mediante http y mediante https a los sitios seguros desde el propio servidor y
desde un cliente W7, aceptando los posibles problemas con la entidad certificadora

![11](img/seguras/22.png)

> Si accedemos por http, nos saldra la página por defecto de nuestro dominio no la configurada por https

![12](img/seguras/23.png)

![13](img/seguras/24.png)

----

#### Carpetas Privadas

* Necesitamos crear una carpeta empleados (dentro de miEmpresa) y, dentro de esta, tres o
cuatro subcarpetas personales con nombres de empleados y una, denominada común, a la que
tendrán acceso todos los empleados, pero no otros usuarios sin identificar.

![1](img/privadas/1.png)

![2](img/privadas/2.png)

![3](img/privadas/3.png)

* Para el sitio web creado y para cada una de sus carpetas, deshabilitamos el acceso anónimo.
* Agregar función de Autenticación Básica a nuestro Servicio de IIS a través de la Administración
del Servidor.

![4](img/privadas/4.png)

![5](img/privadas/5.png)

* En Active Directory, crearemos un usuario para cada empleado (tantos como carpetas
personales) y un grupo Empleados que los incluya a todos.

![6](img/privadas/6.png)

* Configuramos permisos

![7](img/privadas/7.png)

![8](img/privadas/8.png)

![9](img/privadas/9.png)

* Comprobamos el acceso, tanto desde el servidor como desde el cliente W7, a las diferentes
carpetas con distintos usuarios.

![10](img/privadas/10.png)

![11](img/privadas/11.png)

![12](img/privadas/12.png)
