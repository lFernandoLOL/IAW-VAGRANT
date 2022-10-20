# SERVIDOR APACHE Y SQL

## Lo primero es agregar el aprovisionamiento a ambas maquinas

![](/imagenes/APROVISIONAMIENTO_SQL.png)

![](/imagenes/APROVISIONAMIENTO_APACHE.png)

## Ahora creamos el vagrantfile y las maquinas usando los sh de aprovisionamiento

![](/imagenes/VAGRANTFILE.png)

## Hacemos un vagrant up para levantar las maquinas

![](/imagenes/esperamos.png)


## Entramos en el archivo de configuracion de sql para poner la ip de nuestra maquina y se pueda conectar desde apache

![](/imagenes/sqlip.png)
![](/imagenes/IP.png)

## Ahora volvemos a entrar en sql y vamos a crearle un usuario con la ip de apache para que pueda acceder. En mi caso le voy a conceder todos los privilegios en el caso que lo necesite

![](/imagenes/volvemos.png)
![](/imagenes/Basedato.png)



## A continuacion vamos a la carpeta home e importamos la base de datos de josejuan

![](/imagenes/josejuan.png)

## Quitamos los usuarios que creo jose juan para que no hayan errores

![](/imagenes/nano.png)
## Importamos su database

![](/imagenes/Cap.png)


## Por ahora dejamos el servidor sql y vamos a apache...

![](/imagenes/ahora.png)

## Creamos una carpeta en www y clonamos en esta la basededatos
![](/imagenes/cap2.png)

## Comprobamos que estan los archivos que necesitamos para acceder de forma remota a la bd. Estos los vamos a mover a la carpeta "clona" para tenerlos a mano y poder ponerle la configuracion.
![](/imagenes/cap3.png)

## Creamos nuestro propio archivo de configuracion en sites available y lo activamos. Tambien hay que desactivar el que viene por defecto para no incurrir en superposiciones
![](/imagenes/www.png)

![](/imagenes/comprobar.png)


## Ahora vamos al fichero de configuracion de la carpeta activa, y vamos a poner nuestra ip y datos para acceder a sql

![](/imagenes/configphp.png)


## Y por fin vamos a conectarnos a sql con el user apache
![](/imagenes/users.png)


## Vamos a conectarnos desde apache

![](/imagenes/conexion.png)