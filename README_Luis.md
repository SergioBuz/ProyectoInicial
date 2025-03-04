# Proyecto colaborativo en GitHub - Luis Rubio

## Parte común a todos los miembros
Para poder empezar a trabajar, primero debemos <ins>crear un repositorio local</ins>, con la siguiente estructura:
- Archivo index.html en la raíz del repositorio.
- Carpeta CSS con archivo estilos.css en su interior.
- Carpeta JavaScript con archivo mijava.js en su interior.  

Una vez creada la estructura, creamos el repositorio, <ins>añadimos los archivos</ins> a éste y realizamos un <ins>primer commit</ins>.
- Creación del repositorio: ***git init***
- Seguimiento de archivos y directorios: ***git add .***
- Primer commit: ***git commit -m "Commit inicial"***

Creamos un repositorio remoto desde GitHub, y los asociamos mediante el comando:  
***git remote add origin https://github.com/SergioBuz/ProyectoInicial.git***


Ahora <ins>subimos el repositorio local</ins> a GitHub mediante ***git push -u origin master***

El siguiente paso es <ins>añadir colaboradores</ins> en nuestro proyecto de GitHub.
- En tu perfil de GitHub, vas a *Settings>Collaborators* (Opciones>colaboradoes).
- Allí te permite buscar y añadir al usuario que desees. 
- Este recibirá un correo de confirmación y, en cuanto confirme, será colaborador del repositorio.


> [!NOTE]
> Como referencia, Sergio ha sido quien ha creado el repositorio inicial



## Parte personal

De vuelva a Git, creamos una <ins>rama con nuestro nombre</ins> para trabajar sobre ella:  
***git branch Luis  
git switch Luis***

Ya en mi rama personal, procedo a trabajar. Siguiendo un proceso similar al inicial:
- Realizamos un commit con ***git commit -m “Añadido el botón y su funcionalidad en JS y CSS”***
- Actualizamos la rama main para que tenga los últimos cambios con ***git pull origin main***
- Cambiamos a la rama main y traemos los cambios de la rama personal con ***git switch main*** y ***git merge Luis***


Para llevar a cabo el <ins>pull request</ins>, podemos hacerlo gráficamente desde GitHub o con comandos mediante Git.

En el primer caso, simplemente accedemos a la pagina de nuestro pull request y en el fondo encontraremos un botón verde que dice "Merge pull request".

Si preferimos hacerlo en Git, debemos seguir los siguientes pasos:
- Actualizar nuestro repositorio local con los últimos cambios: ***git pull origin Luis***
- Cambiar a la rama del pull request: ***git checkout Luis***
- Hacer un merge con el main: ***git merge main***
- Hacer un push de los cambios: ***git push -u origin Luis***

En caso de <ins>haber conflictos</ins>, tanto GitHub como Git nos avisarán y mostrarán las múltiples opciones para resolverlo.  
En el caso de Git, las opciones del merge se visualizarán mediante nuestro IDE por defecto (VS Code).  
Si todo ha ido bien, se realizarán los cambios y los cambios de nuestra rama se aplicarán al main.  

## Conflictos y problemas

Hemos aprendido a base de prueba y error.  
Los conflictos en merges de la misma rama han sido resueltos sin gran problema.  
El merge entre la rama de Sergio y el main eliminó algunos archivos que no existían en su rama, como este mismo readme que estás leyendo ahora.
A partir de ello, aprendimos que hay 3 modalidades de merge en el pull request... y que se pueden revertir cambios con ***git reset***
