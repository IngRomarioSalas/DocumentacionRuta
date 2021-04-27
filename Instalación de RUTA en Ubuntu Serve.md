# Instalación de RUTA en Ubuntu Server
### By: ***Ing. Romario Salas Diaz*** 
En este manual se presenta una guiá paso a paso para la instalación de RUTA en UBUNTU SERVER, con el fin de optimizar los tiempos de instalación de RUTA.
**RUTA** es un proyecto de juegos para casino, que cuenta actualmente con 6 tipos de juegos.

# Sistema operativo Ubuntu Server 20.04
Este sistema operativo funciona  de manera excelente para el proyecto de ruta, por su facil soporte y aprovechando que es un sistema livianos el cual necesita poco recursos para su funcionamiento.

- **RAM:** 1Gb
- **Disco:** 5Gb

# Entorno de escritorio seleccionado
Para el uso del sistema se hace necesario de un entorno de escritorio, un entorno de escritorio es un conjunto de software que ofrece al usuario una interacción amigable y cómoda. Mientra el entorno tengas mas estilos y mas software por defecto hace que necesite mas memoria y almacenamiento, debido a esto se opto por utilizar openbox.
**Openbox**
Es un entorno de escritorio más ligero que LXDE y Xfce debido a su diseño y apariencia minimalista. Se trata de un entorno de escritorio altamente configurable y tiene un escritorio completamente plano que hace que el proceso de carga sea bastante rápido. Para abrir el menú basta con dar Clic derecho en cualquier lugar en el escritorio.

## Intalar Ubuntu Server
### Paso 1: Buscar la ISO
Para encontrar la iso del sistema operativo ubuntu server se debe ingresar a la pagina oficial de ubuntu y en la parte de descarga elegir ubuntu server o ingresar en el siguiente  enlace  https://ubuntu.com/download/server.
- Click en la opcion2: Instalacion manual.
- Click en descargar Ubuntu Server

### Paso 2: Crear una memoria booteable
Para este paso necesitamos una memoria USB que tenga una capacidad de 4 GB o superior e instalar el programa para crear la memoria booteable, para el proceso de esta guia uso el programa balenaEtcher, el cual es facil de instalar y de usar. 
Este programa se puede conseguir en su sitio oficial https://www.balena.io/etcher/
- Click en descargar
- Instalar y luego lo abrimos.

En el primer campo seleccionamos la iso que se desea instalar en la memoria, en el segundo la memoria y se presiona en “Flash!” luego sería esperar hasta que este lista.

### Paso 3: Instalación del sistema operativo 
Para instalar el sistema operativo conectamos la memoria en cualquier puerto USB y prendemos el equipo, se debe presionar la tecla “F11” para elegir con cual disco iniciar, se selecciona la memoria USB y seguido instalar Ubuntu Server.

**Interfaz de instalación**
- Seleccionar idioma (español)->Enter en "hecho".
- Configurar Teclado (Detectar automaticamente o escoger su configuracion si ya la conoce).->Enter en "hecho".
- Conexiones de RED, verificar que el equipo esta conectado a internet->Enter en "hecho".
- Configuracion de proxy->Enter en "hecho".
- Configuracion de espejo de arhivos de ubuntu(dejar como esta)->Enter en "hecho".
- Configuracion de almacenamiento guiada (dejar como esta)->Enter en "hecho".
- Configuracion de almacenamiento(dejar como esta)->Enter en "hecho".
- Cofiguracion de perfil(nombre(ruta), nombre del servidor(ruta), nombre de usuario(ruta), contraseñas(ruta123*.*))->Enter en "hecho".
- Configuracion de SSH(dejar como esta)->Enter en "hecho".
- Snaps recomendados del servidor(dejar como esta)->Enter en "hecho".
- Se ejecutara la instalacion y luego esperar en la parte inferior cuando salga reiniciar ahora->Enter en "reiniciar ahora".


## Instalar RUTA

# Ubuntu Server 20.04 LTS
## Inicio
Desde que se presiona *el botón de arranque* hasta que aparece la *vista del lanzador* el sistema toma un tiempo de *dos minutos con cuarenta segundos (2.40seg)*
## Tabla de comportamiento



**Aplicación**|**CPU inicial(%)**|**CPU estable(%)**|**CPU max(%)**|**RAM inicio(Gb)**|**RAM 15min(Gb)**|**Tiempo 1ra vez (seg)**|**Tiempo Después (seg)**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Lanzador||63||2,18||||
|Dados|140|140|155|2,77|3,8|9|3|
|Lanzador||63||2,2||||
|BlackJack|192|100|114|2,49|3|6|3,5|
|Lanzador||53||2,23||||
|Ruleta|183|120|150|2,69|3,3|6|3|
|La24|154|138|143|2,69|3,6|6|3|
|Poker|225|115|229|2,7|4,2|11|3|



|**Ubuntu Server**|**Xubuntu**|
| :-: | :-: |
|Fácil de instalar |Fácil de instalar|
|Interfaz lo necesario|Mejor interfaz grafica|
|Ejecuta los procesos rápidos por lo ligero que es |Mas lento al ejecutar procesos|
|Lanzador RAM:2,16 CPU:53%~63%|Lanzador RAM:2,16 CPU:65%~70%|
|BlackJack  RAM:2,49 CPU:100%~114%|BlackJack  RAM:2,50 CPU:100%~140%|
|Ruleta RAM:2,69 CPU:120%~150%|Ruleta RAM:2,78 CPU:110%~179%|

||||**Sistema**|**Operativo**||
| :- | :- | :-: | :-: | :-: | :-: |
|**Ejecución**|**Proceso**|**Ubuntu Server**|**Xubuntu**|**Ubuntu Server**|**Xubuntu**|
|Encendido|Tiempo de encendido(seg)|2,40|2,37|  | ✓ | 
|Lanzador|CPU(%)|53-63|65-70| ✓ | |
||RAM(Gb)|2,18|2,16| | ✓ | 
|Blackjack|Tiempo 1ra vez(seg)|6|5,59| | ✓ | 
||Tiempo despues(seg)|3,5|3,66| ✓ | |
||CPU(%)|100-114|100-140| ✓ | |
||RAM(Gb)|2,49|2,50| ✓ | |
|Ruleta|Tiempo 1ra vez(seg)|6|7,48| ✓ | |
||Tiempo despues(seg)|3|3,50| ✓ | |
||CPU(%)|120-150|110-179| ✓ | |
||RAM(Gb)|2,69|2,78| ✓ | |
|Dados|Tiempo 1ra vez(seg)|8.78|8.83| ✓ | |
||Tiempo despues(seg)|3|3.71| ✓ | |
||CPU(%)|120-155|100-144|  | ✓ | 
||RAM(Gb)|2.77|2.9| ✓ | |
|La24|Tiempo 1ra vez(seg)|6|7.34|✓ | |
||Tiempo despues(seg)|3|3.73|✓ | |
||CPU(%)|130-153|130-160|✓ | |
||RAM(Gb)|2.69|2.89|✓ | |
|Poker|Tiempo 1ra vez(seg)|11|9.32| | ✓ | 
||Tiempo despues(seg)|3|3.37|✓ | |
||CPU(%)|115-229|90-276|✓ | |
||RAM(Gb)|2.7|3.14|✓ | |
|Rieles|Tiempo 1ra vez(seg)|3.50|3.62|✓ | |
||Tiempo despues(seg)|2.11|3.23|✓ | |
||CPU(%)|45-215|70-210|✓ | |
||RAM(Gb)|2.70|2.97|✓ | |
||||**Total**|22 (81.48%)|5 (18.52%)|



## Instalación del entorno de trabajo
Se va ha realizar las instalaciones que corresponde al entorno de escritorio, un gestor de sesión, y programas que se van a usted como complemento
### Instalación de aptitude
Aptitude es un comando sirve para conocer las dependencias que necesita un programa para su instalación y también para consultar si esta instalado o no. Se usara mas adelante cuando se requiero la instalación de cierto paquetes y librerías.
Para instalar el aptitude se debe ingresar al usuario **root**, para eso se utiliza el comando
```sh
#Ingresar al usuario root
sudo su
```
Cuando se utiliza el comando sudo, el sistema pide la contraseña del usuario que se agrego al instalar
el sistema operativo. En el caso actual la contraseña es: ruta123*.*
Para diferenciar si esta como usuario root, primero el nombre del usuario cambia de ruta a **root**, y el simbolo de $ cambia a #.
Para instalar aptitude se introduce el comando
```sh
#Instalar el comando aptitude
sudo apt install aptitude
```
Ya con aptitude se puede tener una mejor instalación de programas, desde ahora se utilizará aptitude para la mayoría de instalaciones. 
Para salirse del modo root se introduce el comando
```sh
#Salirse del usuario root
exit
```
### Instalar pcmanfm
Es una aplicación de gestión de archivos.
```sh
#Instalar pcmanfm
sudo aptitude install pcmanfm
```
### Instalar de openbox
```sh
#Instalar openbox
sudo aptitude install openbox
```
### Instalar obconf
Es un programa creado para Openbox que permitirá no sólo configurar las ventanas de Openbox sino que también se podrá instalar temas para el gestor de ventanas o configurar los lanzadores.
```sh
#Instalar obconf
sudo aptitude install obconf
```
### Instalar terminal
Para la ejecución de los comando dentro de openbox se necesita una terminal, para el caso del manual se va ha usar la terminal de gnome
```sh
#Instalar gnome-terminal
sudo aptitude install gnome-terminal
```
### Instalar lightdm
Lightdm es un gestor de sesiones. La parte visible del gestor de sesiones es la pantalla de bienvenida o de autenticación donde se introduce el login y se puede configurar ciertos parámetros de la sesión.
```sh
#Instalar lightdm
sudo aptitude install lightdm
```
En el proceso de instalación de lightdm se pregunta si quiere usar la interfaz de **gnome** o la de **lightdm**, se elige la opción lightdm y cuando se termine la instalación se reinicia el computador.
```sh
#Reiniciar el sistema
reboot
```
Se inicia por openbox y se abre una terminal
### Desinstalando los entornos de escritorio default
Para conocer los entorno de escritorios actuales
```sh
#Sesiones del sistema
ls /usr/bin/*session
#Para quitar los entornos de escritorio
sudo apt purge –auto-remove gnome-session
```
### Instalación de complementos
#### x11-xserver-utils
Es un programa que interactuá con un servidor de x, mediante dispositivos de entrada y salida como una tarjeta gráfica, monitor, teclado y dispositivo apuntador.
```sh
#Instalar x11-xserver-utils
sudo apt install x11-xserver-utils
```
#### firefox
Es un navegador web que permitirá hacer consulta y hacer descargar de programas más adelante.
```sh
#Instalar firefox
sudo apt install firefox
```
### Archivo sudoers
El archivo sudoers es un archivo que lista los usuarios que tiene privilegios y cuales son sus privilegios.
```sh
#Abrir el archivo sudoers
sudo nano /etc/sudoers
```
Se le debe agregar la siguiente linea
**ruta ALL=(ALL:ALL) ALL**
### Autologin
Para la maquina es sumamente importante que cuando se encienda ingrese sola a la sesión, debido a que el usuario no va ha tener como ingresar la contraseña, y por otro lado tampoco debería ser
necesario que la conozca.
```sh
#Crear el archivo autologin
sudo nano /etc/lightdm/lightdm.conf
```
Dentro del archivo debe estar el contenido
**[SeatDefaults]
autologin-user=ruta
autologin-user-timeout=0**
## Crear el archivo 10_ies.rules
El archivo 10_ies.rules tiene la configuración para que el sistema reconozca los joystick que usa la maquina en donde funciona ruta.
```sh
#Crear el archivo autologin
sudo nano /etc/udev/rules.d/10_ies.rules
```
Se ingresa
##### KERNEL=="js*", SUBSYSTEM=="input", ATTRS{idVendor}=="0079", ATTRS{idProduct}= ="0006", SYMLINK+="ies/key%n", MODE:="0666"
## Instalacion de docker 
Docker es un proyecto de código abierto que automatiza el despliegue de aplicaciones dentro de contenedores de software.
Para la instalación de Docker Engine en el sistema operativo ubuntu se puede guiar de la documentación oficial en https://docs.docker.com/engine/install/ubuntu/
## Instalación de docker-composer
Para la instalacion del docker-compose se
puede guiar del sitio oficial https://docs.docker.com/compose/install/ en el manual se muestra la forma en la que se instaló en el mini-computer
## Instalacion de Qt
Qt es un framework basado en c++ que extiende las funcionalidades del lenguaje de programacion, es multiplataforma orientada a objetos usado para desarrollar programas que utilicen interfaz gráfica de usuario (conexión de los juegos con periféricos de la maquina).
### Pasos para la instalacion de Qt
- Se ingresa al siguiente link **https://www.qt.io/download-qt-installer?hsCtaTracking=99d9dd4f-5681-48d2-b096-470725510d34%7C074ddad0-fdef-4e53-8aa8-5e8a876d6ab4**
- Permisos al archivo que se descargó
```sh
#Dar permisos de ejecución
sudo chmod +x qt*.run
```
- Ejecutar el archivo 
```sh
#Ejecutar el archivo 
./qt*.run
```
- Ingresar credenciales
- Elegir la opcion (I have read and approve...)
- Siguiente
- Elegir la opción (Help us to improve...)
 
El siguiente paso es dar la ubicación en donde va ha quedar el Qt, esta direccion es **~/Documents/qt**
La carpeta qt no esta creada así que esta se debe crear en la dirección. y seleccionar la opción que dice (Custom installation)
- Para el siguiente es señalar unicamente archive(si hay otra seleccionada se quitan) y dar en filter. Se espera que termine la carga y se señala la opción **Qt 5.9.2** que esta en la carpeta Qt
- Ya los otros solo se presionan siguiente hasta que se termine su instalación.

## Anydesk
AnyDesk es un programa de software de escritorio remoto.
### Instalar anydesk
Para instalar el software anydesk se siguen las intrucciones del siguiente link http://deb.anydesk.com/howto.html
### Configuración del Anydesk
Para la configuración de anydesk es necesario ingresar como usuarios **root**
```sh
#Ingresar a la configuración del anydesk
sudo su
anydesk-global-settings
```
Se habilita la opción que dice **"enable unattended access"**, y se le asigna la contraseña: ruta123*.* 
Es muy importante esta opción ya que se usa para revisar el funcionamiento de las maquinas y estas no siempre estan cerca, inclusive puede que ni esten en la misma ciudad.
## Instalar mysql y librería
### Instalar mysql
Mysql es un motor de base de datos SQL.
```sh
#Actualizar repositorio
sudo apt update
#Instalar 
sudo apt install mysql-client
```
### Instalación de la libreria libmysqlclient
Es una librería que se necesita
```sh
#Descargar libmysql
wget https://repo.mysql.com/apt/ubuntu/pool/mysql-5.7/m/mysql-community/libmysqlclient20_5.7.33-1ubuntu18.04_amd64.deb
#Para instalar la configuración
sudo dpkg -i libmysqlclient20_5.7.33-1ubuntu18.04_amd64.deb
#Actualizar repositorios
sudo apt update
#Instalar libreria
sudo apt install libmysqlclient20
```
## Instalar psmisc
El paquete psmisc contiene programas que ayudan al manejo del directorio /proc.
Fuser – identifca procesos mediante archivo o sockets
killall – mata los procesos por nombre
pslog – Imprime la(s) ruta(s) de registro de un proceso.
Entre otros.
```sh
#Instalar psmisc
sudo aptitude install psmisc
```
## Archivos de ruta
### autostart
Es el archivo que se encarga de ejecutar el lanzador cuando se inicia la maquina, el archivo debe estar ubicado en **~/config/openbox/**. pero como la carpeta no existe se debe crear
```sh
#Crear carpeta openbox
mkdir ~/.config/openbox
#Mover el archivo autostart
mv autostart ~/.config/openbox/
```
El archivo debe tener como propietario y grupo a **ruta** y adicional permisos de ejecución para todos los usuarios.
```sh
#Cambio de propietario y grupo
sudo chown ruta:ruta ~/.config/openbox/autostart
#Permisos de ejecución
sudo chmod +x ~/.config/openbox/autostart
```
### Carpeta de RUTA
La carpeta debe moverse a la carpeta principal (~), se le debe dar como propietario y grupo a **ruta**
```sh
#Cambio de propietario y grupo
sudo chown ruta:ruta RUTA
#Mover el directorio RUTA a (~)
sudo mv RUTA ~/
```
En esta carpeta estan los lanzadores y los juegos, asi que necesitan permisos de ejecución.
```sh
#Permisos de ejecucion a los juegos
sudo chmod +x /home/ruta/RUTA/*/*.x86_64
#Todos los permisos a los .xml
sudo chmod 777 /home/ruta/RUTA/*/*/*/*.xml
```
Entro del directorio RUTA se debe crear un directorio llamado db, este debe pertenecer a 999 y tener como grupo a docker
```sh
#Crear directorio
sudo mkdir /home/ruta/RUTA/db
#Cambio de propietario y grupo
sudo chown 999:docker /home/ruta/RUTA/db
```
Y por último se crea la carpeta **Screenshots** dentro de la carpeta
```sh
#Crear directorio
sudo mkdir /home/ruta/RUTA/Screenshots
```
### Carpeta docker
La carpeta de docker debe moverse a **~/Documents**
```sh
#Cambio de directorio
mv docker ~/Documents/
```
### Archivos configuration manager genericModals docker-clean
los archivos van ubicados en **/usr/local/bin**, deben tener **permisos de ejecución**, pertenecer y tener como grupo a **ruta**
```sh
#Cambio de directorio
sudo mv configuration manager genericModals docker-clean /usr/local/bin/
#Permisos de ejecución
sudo chmod +x /usr/local/bin/*
#Cambio de propietario
sudo chown ruta:ruta /usr/local/bin/*
```
### Archivo ttys-enable.service y ttys-enable.sh
El archivo **ttys-enable.service** se debe mover a **/etc/systemd/system/** y el archivo **ttys-enable.sh** se debe mover a **/usr/bin/**. Ambos archivos deben de tener como propietario y grupo a root y permisos de ejecución
```sh
#Cambio de propietario
sudo chown root:root ttys-enable*
#Permisos de ejecución
sudo chmod +x ttys-enable*
#Cambio de directorio
sudo mv ttys-enable.sh /usr/bin/
sudo mv ttys-enable.service /etc/systemd/system/
#Ir a la carpeta /etc/systemd/system/
cd /etc/systemd/system/
#Correr service
sudo systemctl enable ttys-enable.service
#Comenzar el servicio
sudo systemctl start ttys-enable.service
```
### Archivo billetero.ini
El archivo debe estar ubicado en **/etc/ruta** Pero antes de moverlo se debe de crear el directorio ruta.
Adicional el archivo necesita todos los permisos y tener como propietario y grupo a **ruta**
```sh
#Crear directorio ruta
sudo mkdir /etc/ruta
#Todos los permisos
sudo chmod 777 billetero.ini
#Cambio de propietario y grupo
sudo chown ruta:ruta billetero.ini
#Cambio de directorio
sudo mv billetero.ini /etc/ruta/
```
### Archivo de autoverificacion.sh
Debe pertenecer y tener como grupo a **root**, estar ubicados en **/usr/bin/** y tener permisos de ejecución
```sh
#Cambio de propietario y grupo
sudo chown root:root autoverificacion.sh
#Permisos de ejecución
sudo chmod +x autoverificacion.sh
#Cambio de directorio
sudo mv autoverificacion.sh /usr/bin/
```
### Archivo crontab
Al archivo crontab se le debe agregar la linea 
01 * * * * root find /RUTA/Screenshots/* -mtime +1 -delete
```sh
#Abrir el archivo crontab
sudo nano /etc/crontab
```
### kbitech_ICT
La carpeta debe tener **todos los permisos**, pertener a **root** y estar en **/usr/include/**
```sh
#Permisos de ejecución
sudo chmod 777 kbitech_ICT
#Cambio de propietario y grupo
sudo chown root:root kbitech_ICT
#Cambio de directorio
sudo mv kbitech_ICT /usr/include/
```
### Carpeta Barra de carga
La carpeta se de ubicar en el directorio **~/** y se le debe cambiar el nombre a **imagenes**
```sh
#Cambio de nombre y directorio
sudo mv Barra\ de\ carga/ ~/imagenes
```
### Archivos libITC_Bill
Los archivos libITC_Bill deben tener como propietario y grupo a **root**, debe tener permisos de **ejecución** y estar ubicados en la dirección **/usr/lib/**
```sh
#Permisos de ejecución
sudo chmod +x libICT_bill.s*
#Cambio de directorio
sudo mv libICT_BILL.so* /usr/lib/
```
## Instalar librerías necesarias para manager configuration genericModals
Para el funcionamiento de los archivos ya mencionados se necesitan unas librerías adicionales
```sh
#Librerias para manager
sudo aptitude install libqt5printsupport5
sudo aptitude install libqt5serialport5
sudo aptitude install libqt5websockets5
#Librerias para configuration
sudo aptitude install libqt5sql5
#Librerias para genericModals
sudo aptitude install libqt5quick5
sudo aptitude install qml-module-qtmultimedia
sudo aptitude install qml-module-qtquick-window2
```
Como complemento se instalan tres programas más
**feh**
Es un visor de imágenes ligero dirigido principalmente a usuarios de interfaces de línea de comandos.
**wmctrl**
Es un comando que permite interactuar con una ventana x
**alsa-utils**
Es un programa para manipular los sonidos.
```sh
#Instalar feh
sudo apt install feh
#Instalar wmctrl
sudo aptitude install wmctrl
#Instalar alsa-utils
sudo apt-get install alsa-utils
```
## Ejecutar archivos de docker
Se necesita construir y desplegar los contenedores de docker
```sh
#Cambiar al directorio de docker 
mv ~/Documents/docker
#Construir los contenedores
sudo docker-compose -f docker-compose.yml build
#Desplegar los contenedores
sudo docker-compose -f docker-compose.yml up -d
```
## Instalar ssh
Es un programa que sirve para controlar de forma remota la terminal, lo que va ha servir para observar el comportamiento de la maquina.
```sh
#Instalar openssh-server
sudo aptitude install openssh-server
#Instalar openssh-client
sudo aptitude install openssh-client
```





