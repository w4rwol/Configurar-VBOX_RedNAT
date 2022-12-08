# CONFIGURACIÓN RED NAT
Nuestro objetivo es conectar tres máquinas virtuales dentro de una misma red NAT y establecer conexión a internet entre ellas.

INTERFACES
Una vez hayamos instalado en Virtual Box los S.O Windows 10, Windows Server 2019 y CentOS, debemos crear una red NAT.
Accedemos a `VirtualBox --> Archivo --> Herramientas --> Network Manager`
En la nueva ventana, abrimos la pestaña de `NAT Networks` y creamos una nueva red con el nombre que queramos.

img1

Una vez creada la red NAT,  hay que asignarla a las tres máquinas.
Seleccionamos la máquina que queramos, abrimos su configuración y, dentro de `Red`, cambiamos el adaptador 1 de `NAT` a `Red NAT` y así con todas.

Es importante que todas estén dentro de la misma red NAT para poder hacer ping y encontrarse.

img2

# CONFIGURAR LA IP

Ahora, debemos ver la nueva red que hemos asignado a cada una de las máquinas, con los comandos `ipconfig` y `ifconfig`, dependiendo del S.O.

## Windows 10


## Windows Server 2019


## CentOS 7



