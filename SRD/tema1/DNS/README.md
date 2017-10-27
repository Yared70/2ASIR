# Instalación y configuración de un servidor DNS

#### Se piden las siguientes acciones de configuración y prueba del funcionamiento del servicio:

> * Crear una zona de búsqueda directa para tu servidor.
> * Crear una zona de búsqueda inversa para tu subred.
> * Configurar reenviadores DNS

![1](img/1.png)

    Seleccionamos crear una zona directa e inversa

![2](img/2.png)

![3](img/3.png)

![4](img/4.png)

![5](img/5.png)

![6](img/6.png)

    Creación de la zona interna

![8](img/8.png)

![9](img/9.png)

Aqui configuramos los reenviadores

![7](img/7.png)

> Una vez hecho esto, en el cliente asignamos al server como dns y comprobamos su funcionamiento

![10](img/-6.png)

![11](img/-9.png)

**En la zona de búsqueda directa añadir los siguientes registros:**

> * Un alias para tu servidor denominado server.
> * Una impresora con IP fija denominada printer (no hace falta alias).
> * Un servidor de correo (ficticio) denominado correo, asociado a una dirección en tu servidor.
> * Crear una subzona denominada servicios (dominio nuevo) y agregar a ésta un servidor ftp (asociado a la misma IP del servidor), una impresora nueva (con una IP fija) y el equipo del administrador del sistema (también con IP fija).

* **Server**

![12](img/-10.png)

* **Printer**

![13](img/-11.png)

* **Servidor**

![15](img/-13.png)

* **Nuevo dominio: servicios**

![16](img/-14.png)

![17](img/-16.png)

> * Comprobar que se resuelven los nombres desde la consola del servidor.

![18](img/-17.png)

> * Validar un cliente en el dominio y comprobar que el nombre de su equipo aparece en la zona de búsqueda del servidor como un nuevo registro A

![19](img/-18.png)

![20](img/-19.png)

> * Realizar, también desde el cliente, algunas operaciones con nslookup

![21](img/-20.png)

![22](img/-21.png)
