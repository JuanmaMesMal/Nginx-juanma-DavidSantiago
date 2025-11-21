# Instalacion servidor web Nginx    
- Para esto vamos a crear el debian, usaremos el trabajo de dns-paso-paso como base del proyecto.

## Instalacion servidor web Nginx
- Instalamos el servidor en la maquina virtual (con el comando sudo apt update e install).
![IsntalarServidor](assets/img/sudoAptUpdate.PNG)
- Creamos las carpetas donde se localizara el sitio web en nuestro caso pondremos var/www/juanma-davidS.test/html.
![Creacion Carpetas](assets/img/crearCarpetas.png)
- Clonamo desde github una website
![Clonar github](assets/img/FalloGitClone.png)
  - Nos sale un fallo, cual nos dice que no tenemos instalado git, y luego nos da otro fallo por permisos (se puede arreglar cambiando los permisos o accediendo a root)
![Clonar github nice](assets/img/GitCloneNice.png)
- Ahora necesitaremos añadirle permisos a esta carpeta, y abrimos la pagina web desde un navegador poniendo la ip de la maquina.
![Permisos](assets/img/Permisos.png)
![Web Ip](assets/img/PaginaWeb.png)

- Creo un bloque de servidor con las directivas correctas.
![Crear Nano](assets/img/CrearNanoRuta.png)

- Creamos un archivo simbolico para dar de alta automaticamente y reiniciamos.
![Crear archivo](assets/img/ArchivoSimbolico.png)

## Comprobar funcionamiento

- Para hacerlo sin dns, hay que abrir bloc de notas como administrador, con esta ruta C:\Windows\System32\drivers\etc\hosts, y al final añadimos nuestra ruta, en n uestro caso es 192.168.56.10   juanma-davids.test
![Sin DNS](assets/img/SinDNS.png)