### Examen 1
**Universidad ICESI**  
**Curso:** Sistemas Operativos  
**Docente:** Daniel Barragán C.  
**Tema:** Comandos de Linux, Virtualización  
**Nombre:** Carlos Andrés Torres López  
**Código:** A00141804


Parcial Sistemas operativos  

3.  
 1.	Sum_all_numbers  

Respuesta:  
-	Como primer paso creo un archivo sumar.txt dentro del directorio Home.  
-	En el archivo ingrese los números por línea 1,2,3,4.  
-	Luego de esto descargue bc con el comando yum install bc  
-	Luego de esto ejecuto el siguiente comando paste –sd+ sumar.txt | bc  lo que da como resultado la suma de los números, presento a   continuación el pantallazo:  

 ![sumar](https://github.com/candrelopez/so-exam1/edit/A00141804/sumar.jpg)  
 

2.	replace_spaces_in_filenames  

Respuesta:  
-	Inicialmente creo el archivo readme.txt con la siguiente información:  

 

Posteriormente utilizo el comando sed  de la siguiente manera sed –i –e  ‘s/ /g’ mas el nombre del fichero en este caso readme.txt y   esto modifica el archivo de la siguiente manera:  

 

Dando como resultado:

 




3.	reverse_readme

Respuesta:
Cree el archivo readme.txt con la siguiente información:

 

Luego utilizo el comando tac  de la siguiente manera tac readme.txt y genera lo siguiente:

 

4.	remove_duplicated_lines  
Respuesta:  
Inicialmente creo un archivo que se llama líneas repetidas con la siguiente información:  
 
 Luego de esto utilizo el el siguiente comando cat líneas_repetidas.txt | sort | uniq lo que me genera el siguiente resultado:  

 
Claramente se ve como quita las líneas repetidas.  
5.	Disp_table  
Respuesta:  

Par imprimir las líneas del archivo csv utilizo la siguiente línea de comando:  
 

Y tiene como resultado:  

 


4.  Para iniciar con la creación del script realizo lo siguiente:  
Primero creo el usuario gutnberg con el comando:  
-	Useradd –m Gutenberg  
Luego de crear el usuario dentro de la su directorio creo el directorio mybooks   
Con el siguiente comando:  
-	mkdir mybooks  
y dentro de este directorio creo el script.sh de la siguiente forma:  
-	touch script.sh && chmod +x script.sh  
-	luego utilizo el siguiente comando:  
-	echo ‘#!/bin/bash’ > script.sh && echo ‘# -*- ENCODING:  UTF-8 -*-‘ >> script.sh  
Con esto queda creado el script.  
Luego de esto descargo por medio de yum el paquete wget de la siguiente manera:  
Yum install wget  




