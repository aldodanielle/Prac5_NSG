# Practica 5
## NSG (Grupo de Seguridad de Red o Net Segurity Grup)
### Paso 1:
Creamos una Máquina Virtual (VM) y el apartado de Datos Básicos para después pasarnos a el apartado de Redes y lo único que cambiamos en ese apartido es el grupo de seguridad de red NIC a ninguno y también en el apartado de administración deshabilitamos la opción de arranque y por ultimo la revisamos y creamos.

![Imagen 1](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P1.png)
![Imagen 1.1](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P2.png)
--------------------------------------------------------------------------------
### Paso 2:
Nos dirigimos a el Grupo de Seguridad de Red y creamos uno nuevo

![Imagen 2](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P3.png)
--------------------------------------------------------------------------------
### Paso 3:
Entramos al recurso creado (NSG) y nos dijimos a interfases de red y asociamos la nueva interfaz de red de nuestra Máquina Virtual creada anteriormente. 

![Imagen 3](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P4.png)
--------------------------------------------------------------------------------
### Paso 4:
Después no dirigimos a las Reglas de seguridad de entrada y agregamos una nueva y llenamos todos los datos que se necesitan para agregar una nueva regla esto con el fin de poder conectarnos a la Máquina Virtual por RDP ya que anteriormente no nos lo permitía porque no tenía una regla de entrada.

![Imagen 4](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P5.png)
![Imagen 4.1](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P6.png)
--------------------------------------------------------------------------------
### Paso 5:
Regla entrada creada nos tiene que permitir ya la conexión por RDP a la Máquina Virtual y solo basta con descargar el RDP de la máquina, conectarnos y logearnos con nuestro usuario y contraseña. 

![Imagen 5](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P7.png)
--------------------------------------------------------------------------------
### Paso 6:
Una vez que ya nos conectamos es hora de crear una nueva regla de seguridad de salida para ello nos dirigimos a esa configuración y agregamos una nueva con el mismo origen y el mismo intervalos pero en este caso en destino colocamos el servicio de etiquetas para que ningún puerto se pueda salir a Internet y por consecuencia ya no podemos conectarnos a internet.

![Imagen 6](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P8.png)
![Imagen 6](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P9.png)
--------------------------------------------------------------------------------
## NOTA:
Por medio de las reglas de seguridad se pueden bloquea y habilitar y por la IP que nos se conecten incluso que esta máquina que solamente se pueda conecte y pase por el firewall incluso que salga por otra maquina asia internet gracias a la IP publica que los quipos tienen. Y también que se puede bloquear una maquina que se trate de conectar con una prioridad alta.
Dos reglas no pueden tener la misma prioridad y tampoco se pueden deshabilitar solo eliminar.


![Imagen 7](https://github.com/aldodanielle/Prac5_NSG/blob/main/Imgenes/P10.png)
--------------------------------------------------------------------------------
