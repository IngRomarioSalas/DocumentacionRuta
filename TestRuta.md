# Comparar las distribución de Ubuntu Server con Xubuntu
En esta guía se van a comprar las distribuciones de los sistemas ya antes mencionados, con el fin de saber cual es el mejor candido para funcionar con el proyecto de Ruta.
**Ruta** es un proyecto de juegos para casino, que cuenta actualmente con 6 tipos de juegos.
# Xubuntu 20.04 LTS
Xubuntu es una distro de Linux basada en Ubuntu como su propio nombre lo indica, y utiliza el entorno de escritorio XFCE. Está diseñada para usuarios con equipos limitados ya que únicamente necesita.

|      | VALOR |
| ------ | ------ |
| RAM | 1 Gb |
| DISCO | 8 Gb |
| Tamaño de iso | 1.6 Gb |

Este sistema operativo trae muchas cosas que no son necesarias para correr Ruta, como por ejemplo libreoffice, aplicaciones multimedia, entro otras.
El soporte de esta distribucion es de 3 años.
# Sistema operativo Ubuntu Server 20.04 LTS
Este sistema operativo funciona  de manera excelente para el proyecto de ruta, por su facil soporte y aprovechando que es un sistema livianos el cual necesita poco recursos para su funcionamiento.
Es la última versión de este sistema operativo para la creación de servidores Linux. Las versiones LTS del sistema operativo nos aseguran actualizaciones durante 5 años desde su lanzamiento.
|      | VALOR |
| ------ | ------ |
| RAM | 1 Gb |
| DISCO | 5 Gb |
| Tamaño de iso | 1.2 Gb |
## Test de Ruta
## Instalación del sistema Ubuntu Server 20.04 LTS 
El sistema operativo Ubuntu Server se toma aproximadamente **8 minutos** desde el momento en que aparece la vista inicial de la interfaz de instalación hasta que se termina este proceso (Hasta que se reinicia)
Para la parte de las configuraciones iniciales se toma aproximadamente **20 minutos** lo que sería el pcmanfd, el entorno de escritorio hasta llegar a Qt
La instalación de Qt toma **17 minutos** 
La última sesión de instalación toma alrededor de **40 minutos**, en las cuales se instalan docker, librerías, mover archivos, permisos, entre otros.
## Instalación del sistema Xubuntu 20.04 LTS
El sistema operativo Xubuntu se toma aproximadamente **11 minutos** desde el momento en que aparece la vista inicial de la interfaz de instalación hasta que se termina este proceso (Hasta que se reinicia)
Para la parte de las configuraciones iniciales se toma aproximadamente **17 minutos** lo que sería el pcmanfd, el entorno de escritorio hasta llegar a Qt
La instalación de Qt toma **20 minutos** 
La última sesión de instalación toma alrededor de **44 minutos**, en las cuales se instalan docker, librerías, mover archivos, permisos, entre otros.
## Abriendo el juego
Desde que se presiona el botón de arranque hasta que aparece la vista del lanzador el sistema toma un tiempo de dos minutos con cuarenta segundos (2.40seg)

## Tabla de comportamiento

Aplicación|CPU inicial(%)|CPU estable(%)|CPU max(%)|RAM inicio(Gb)|RAM 15min(Gb)|Tiempo 1ra vez (seg)|Tiempo Después (seg)|
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

## Conclusión
Después de analisis de tiempo y según lo datos obtenidos por las tablas comparativos, se a llegado a la decisión de elegir a **Ubuntu Server** como sistema operativo para el software Ruta, debido a que este presenta mas agilidad la mayor parte de sus proceso
