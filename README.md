# Dataset Productos Agrícolas 

* Dataset acerca de Productos Agrícolas implementando MongoDB y MongoDB Compass.
* Esta db ha sido creada utilizando datasets públicos nacionales para poder ser implementado a través de una Api Rest con NodeJs. 
* Link Datasetes públicos : https://www.argentina.gob.ar/economia/politicaeconomica/regionalysectorial/informesproductivos/datasets
* Dataset Tabaco : apróx 5000 registros.
* Dataset Té : apróx 2600 registros.
* Dataset Trigo : apróx 40000 registros.
* Dataset Yerba Mate : apróx 4000 registros.


</br>
 
* Repositorio Api Rest :  


</br>

### Documentación Gráfica de la DB.

</br>

### Colecciones de Datos

![Index app](https://github.com/andresWeitzel/dataset_productos_agricolas_mongodb/blob/master/doc/collections.png)



</br>

### Dataset Tabaco

![Index app](https://github.com/andresWeitzel/dataset_productos_agricolas_mongodb/blob/master/doc/collectionTabaco.png)

</br>

### Dataset Té

![Index app](https://github.com/andresWeitzel/dataset_productos_agricolas_mongodb/blob/master/doc/collectionTe.png)


</br>

### Dataset Trigo

![Index app](https://github.com/andresWeitzel/dataset_productos_agricolas_mongodb/blob/master/doc/collectionTrigo.png)



</br>

### Dataset Yerba Mate

![Index app](https://github.com/andresWeitzel/dataset_productos_agricolas_mongodb/blob/master/doc/collectionYerbaMate.png)



<hr>

## Más Información

</br>


| **Tecnologías Empleadas** | **Versión** | **Finalidad** |               
| ------------- | ------------- | ------------- |
| MongoDB | 5.0  | DB  |
| MongoDB Compass | 1.31.2  | Gestor de MongoDB | 
| Git Bash | 2.29.1  | Control de Versiones |
| CMD | 10 | Manipular los Servicios de Postgres mediante linea de comandos | 

</br>


## Descarga y Documentacion de las Tecnologías Empleadas:

</br>

| **Tecnologías** | **Descarga** | **Documentación** |               
| ------------- | ------------- | ------------- |
| Git Bash |  https://git-scm.com/downloads |   https://git-scm.com/docs |
| MongoDB |  https://www.mongodb.com/try/download/community  | https://www.mongodb.com/try/download/community |
| MongoDB Compass | https://www.mongodb.com/try/download/compass  | https://www.mongodb.com/try/download/compass | 

</br>

## Bibliografía Oficial y No Oficial Recomendada
* Doc oficial : https://www.mongodb.com/docs/manual/tutorial/getting-started/
* Convertidor CSV a Json : https://www.convertcsv.com/csv-to-json.htm




<hr>

## Creación de Documentos/Base de Datos y Colección

* Podemos usar MongoSHELL, pero es poco eficiente y legible la inseción de datos por shell, usaremos Compass (https://www.mongodb.com/products/compass) como interfaz gráfica y editor
* Si se tiene el dataset en formato csv aplicar conversión a formato json. Recomiendo esto para el manejo de los mismos a través de la api.

### Pasos MongoDB

#### Creamos nuestra db
* Database Name : db_productos_agricolas.
* Collections Names : tabaco, te, trigo, yerba-mate

#### Agregar registros desde archivo CSV
* Seleccionamos nuestra db, seleccionamos la colección productos
* ADD DATA
* import file
* select file
* linkeas el doc csv desde el filesystem de este repo
* import
* Si aparecen los registros se ha importado correctamente

</br>



#### Agregar registros desde archivo Json
* En mi caso use un convertidor de documentos online, pase el archivo CSV a JSON. 



</br>


##  Uso y Manejo de Git.

</br>

###  Descarga y Configuración de Git

####  Descarga de Git
* Nos dirigimos a https://git-scm.com/downloads y descargamos el versionador
* Como toda aplicacion siguiente.... siguiente....
* IMPORTANTE:NO TENER DBEAVER ABIERTO DURANTE LA INSTALACION, SINO NO RECONOCE EL PATH

####  Abrir una Consola de Git (Git Bash) desde Windows
* --> Escribimos Git Bash desde el Buscador de Windows
* --> Desde la consola escribimos el comando cd seguidamente de la ruta del proyecto
* --> Tenemos que tener la ruta del Proyecto y pegarla en el Git Bash
* --> Una vez dentro del Proyecto podremos hacer uso de Git

</br>

###  Subir el proyecto al repositorio de github desde la consola de git 

#### Creamos un nuevo repositorio en GitHub.

#### Inicializamos nuestro repositorio local .git desde la terminal.
* git init

#### Agregamos lo desarrollado a nuestro repo local desde la terminal.
* git add *

#### Agregamos lo que tenemos en nuestro repo local al área de Trabajo desde la terminal.
* git commit -m "agrega un comentario entre comillas"

#### Le indicamos a git donde se va a almacenar nuestro proyecto(fijate en tu repositorio de github cual es el enlace de tu proyecto(esta en code)).
* git remote add origin https://github.com/andresWeitzel/dataset_productos_agricolas_mongodb

#### Subimos nuestro proyecto.
* git push -u origin master


</br>


### Actualización del repositorio del proyecto desde la consola de GIT

#### Visualizamos las modificaciones realizadas en local
* git status

#### Agregamos lo modificado al área de trabajo
* git add *

#### Confirmamos las modificaciones realizadas
* git commit -m "tu commit entre comillas"

#### Sincronizamos y traemos todos los cambios del repositorio remoto a la rama en la que estemos trabajando actualmente.
##### (SOLO SI SE REALIZARON CAMBIOS DESDE OTRA LADO, ej: en github u/o/y un equipo de trabajo)
* git pull https://github.com/andresWeitzel/dataset_productos_agricolas_mongodb

#### Enviamos todos los cambios locales al repo en github
* git push https://github.com/andresWeitzel/dataset_productos_agricolas_mongodb

#### En casos extremos pisamos todo el repositorio
* git push -f --set-upstream origin master


