# Resumen - 2da Sesión

* Revisión de lecturas de `Docker`
  * Revisamos modelo de capas de `Docker`
  * Como el modelo de capas de `Docker` tiene un manejo astuto del cache de las imágenes
* Comenzamos a jugar con los [laboratorios](../../laboratorios/)
  * Revisando comandos básicos de Docker
    * `docker images`: lista las imágenes existentes
      * `--help`: help, muestra la ayuda del comando
      * `-a`: all, lista todas las imágenes
      * `-q`: quiet, lista solamente los IDs
    * `docker rmi`: remueve una imagen
      * `--help`: help, muestra la ayuda del comando
    * `docker image rm`: otra forma de remover una image
      * `--help`: help, muestra la ayuda del comando
    * `docker run`: ejecuta/instancia un contenedor
      * `--help`: help, muestra la ayuda del comando
      * `--name`: asigna un nombre al contenedor
      * `-p`: port mapping, asigna un puerto del sistema host al contenedor
      * `-e`: environment variables, crea o asigna valores a variables de entorno que el contenedor puede usar
      * `-d`: daemonizado o detached, corre proceso en el background
      * `--link`: conecta contenedores entre si para que puedan comunicarse (legacy)
    * `docker pull`: descarga imágenes del registro
      * `--help`: help, muestra la ayuda del comando
    * `docker ps`: lista los contenedores en ejecución
      * `--help`: help, muestra la ayuda del comando
      * `-a`: lista todos los contenedores independientemente del estatus
    * `docker logs`: revisar logs de un contenedor
      * `--help`: help, muestra la ayuda del comando
    * `docker inspect`: obtén información del contenedor
      * `--help`: help, muestra la ayuda del comando
      * `-f` o `--format` para formatear la salida usando templates de GO
    * `docker container inspect`: obtén información del contenedor
      * `--help`: help, muestra la ayuda del comando
      * `-f` o `--format` para formatear la salida usando templates de GO
    * `docker stop`: detén contenedores
      * `--help`: help, muestra la ayuda del comando
    * `docker rm`: borra contenedores
      * `--help`: help, muestra la ayuda del comando
  * Jugando con [`laboratorio-1`](../../laboratorios/laboratorio-1/)
    * Creamos los contenedores
    * Nos conectamos a la BD por medio del cliente CLI de `mysql` dentro del contenedor, y por medio de `PHPMyAdmin`
  * Jugando con [`laboratorio-2`](../../laboratorios/laboratorio-2/)
    * Creamos el contenedor de `MongoDB`
    * Nos conectamos a la BD por medio del cliente CLI de `mongo` dentro del contenedor, y por medio de un `DBMS` externo instalado en nuestro sistema host, por ejemplo [`robo3t`](https://robomongo.org/)
    * Corremos los scripts de `Python` anexos, y visualizamos resultados
* Conceptos clave
  * `DBMS`: Manejador de Base de Datos (_DataBase Management System_ por sus siglas en inglés)
  * Revisando tema de puertos de `Docker` y los protocolos que funcionan debajo del mismo. Consultas recomendadas:
    * [Modelo OSI](https://www.ionos.mx/digitalguide/servidores/know-how/el-modelo-osi-un-referente-para-normas-y-protocolos/)
    * [TCP/IP](https://openwebinars.net/blog/que-es-tcpip/)
    * [UDP](https://infotecs.mx/blog/protocolo-udp.html)
