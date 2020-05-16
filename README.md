# Covidmap
# Proyecto Final  Telematica 

Detalles del Estudiante:
Jean pierre agudelo taborda
ID :  400081
Ing. Sistemas
Jhonatan Harold Rueda
ID : 379440
Ing. telecomunicaciones
# DESCRIPCIÓN
Para el desarrollo de la aplicacion usaremos App inventor,
La Aplicación te ayudara a manejar la crisis actual del coronavirus, esta dara información
en tiempo real de los casos en tu zona y usando grafos decir que tan seguro o no es estar en ciertas localidades,
ademas si sientes sintomas , pediremos tus datos como nombre, edad, sexo y si tienes enfermdades base, con esto  recolectaremos los datos 
para asi tener una base de datos mas eficiente.

# Appinventor

En Appinventor sera donde construiremos la aplicación que contara con 3 pantallas la primera estara el menú, en la segunda se pediran los datos al usuario como nombre, edad , sexo , si tiene enfermedades base , si es diagnosticado con covid-19, si el usuario desea la información sera enviada al servidor y se usará en las estadisticas, en la ultima pantalla esta el mapa donde se evidenciaran los casos locales del coronavirus.  


# ARQUICTETURA
<h2>Dockerfile</h2>
El Dockerfile se encargara de montar el servidor, relacionandose con los contenedores; Levantara los servicios necesarios y ejecutará el .py por debajo de memoria y a habilitara el puerto 80 para su uso.

<h2>proyect.py</h2>
  Este sera el archivo principal del proyecto, aqui recibira los datos enviados por el usuario utilizando el metodo POST implementado en 
  la aplicación, ya con sus datos y una base de datos tomada de internet en tiempo real analizaremos la localidad para realizar los graficos y que tan peligroso es estar allí ademas si la persona es diagnosticada con coronavirus o tiene sintomas tambien aparece registrada en los graficos, esto se hara con la ayuda con flask libreria de python 
  
  <h2>BaseDatos</h2>
  
 Esta base de datos tendrá la información de los casos confirmados de covid-19 en Medellín incluyendo los datos dados por los usuarios enfermos o con sospechas. Estos datos son suministrados por internet y mismos usuarios de la aplicación 
 
 # Contenedor en Docker
  Se usara Ubuntu server 18 en el habrá un contenedor, en  este  estaran los archivos, el flask, el pip y python ya estaran instalados ademas el servidor apache, todo previamente actualizado para poder ser usado
  
  # Tipo de Servidor y Firewall
 Se usuará el UFW como el firewall del sistema habilitando el puerto 80. Si el servicio se va montar en una red de servidores en la nube (como AWS) se activara el puerto 22 y se haran las configuraciones de los grupos de seguridad respectivos.




