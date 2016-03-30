# MEDA_Toolbox_GUI
Interfaz gráfica de software libre para la MEDA Toolbox

---- CONTENIDO DEL DIRECTORIO DE DISTRIBUCIÓN ----

MEDA_Toolbox_GUI/

* /Ejecutable_GUI

	- /lib: 	Librerías por defecto utilizadas por la interfaz gráfica (imprescindibles para el funcionamiento)
			Deberán estar incluidas en el mismo directorio en el que se encuentre el ejecutable GUI_MT.jar
	- /src: 	Código fuente, imágenes y archivos originales del JavaDoc de la aplicación 
	- GUI_MT.jar:	Ejecutable Java para iniciar la interfaz gráfica
			Requiere tener en la misma ruta en la que se encuentre el directorio /lib anterior
	- JAVADOC:	Acceso directo a la documentación (JavaDoc) de la aplicación
	- README.TXT:	Fichero de información generado automáticamente con la construcción del ejecutable

* /Ejemplos

	- /Datos_Clase:	Fichero datos_clase.m con las variables y conjunto de datos utilizados en el Apéndice. Manual de Usuario
	- /VAST_2012:	Fichero VAST_2012.m con las variables y conjunto de datos analizados en el Tema 8. VAST Challenge 2012 – MC 2 (Capítulo III) 
			El fichero VAST_2012_ORIG.m contiene los datos originales proporcionados en el reto

* /MEDA_Toolbox

	Funciones que implementan tanto las herramientas de la MEDA_Toolbox ya disponibles, como las funcionalidades creadas específicamente para la interfaz diseñada

* /Octave 3.8.1

	- octave-3.8.1-installer.exe:	Archivo ejecutable de la versión 3.8.1 del software GNU Octave con la que se ha hecho compatible la aplicación
	- ginput.m:			Script de la función principal para la interactuación con los gráficos de dispersión
	- JavaDOC JavaOCTAVE:		Documentación en formato web de la interfaz de comunicación entre Java y Octave



---- PROCEDIMIENTO DE INSTALACIÓN E INICIALIZACIÓN ----

* Entorno de Ejecución de Java

	- Descargar e instalar la última versión del Java SE Runtime Environment

* Octave

	- Lanzar el ejecutable octave-3.8.1-installer.exe situado en la ruta MEDA_Toolbox_GUI\Octave 3.8.1
	- Añadir la ruta C:\<directorio_instalacion>\Octave-3.8.1\bin a la Variable de Entorno Path
	- Copiar el archivo ginput.m situado en el ruta MEDA_Toolbox_GUI\Octave 3.8.1 y sobreescribirlo en C:\<directorio_instalacion>\Octave-3.8.1\share\octave\3.8.1\m\plot\util

* MEDA_Toolbox

	- Copiar la carpeta MEDA_Toolbox_GUI\MEDA_Toolbox en C:\
	  (La interfaz la busca en esa ubicación para ejecutar los scripts contenidos en ella)

* Ejecutable

	- Ejecutar el archivo GUI_MT.jar
	  (Mantener siempre en la misma carpeta este archivo y el directorio MEDA_Toolbox_GUI\Ejecutable_GUI\lib que contiene las librerías necesarias)
