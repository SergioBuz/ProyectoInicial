Para poder empezar a trabajar, primero debemos crear un repositorio local, con la siguiente estructura:
- Archivo index.html en la raíz del repositorio.
- Carpeta CSS con archivo estilos.css en su interior.
- Carpeta JavaScript con archivo mijava.js en su interior.

Una vez creada la estructura, creamos el repositorio, añadimos los archivos a éste y realizamos un primer commit.
- Creación del repositorio: _git init_
- Seguimiento de archivos y directorios: _git add._
- Primer commit: _git commit -m "Commit inicial"_

Creamos un repositorio remoto desde GitHub, y los asociamos mediante el comando:
_git remote add origin https://github.com/SergioBuz/ProyectoInicial.git_


Ahora subimos el repositorio local a GitHub mediante _git push -u origin master_

El siguiente paso es añadir colaboradores en nuestro proyecto de GitHub.
En tu perfil de GitHub, vas a Settings>Collaborators (Opciones>colaboradoes).
Allí te permite buscar y añadir al usuario que desees. 
Este recibirá un correo de confirmación y, en cuanto confirme, será colaborador del repositorio.

De vuelva a Git, creamos una rama con nuestro nombre para trabajar sobre ella:
_git branch Luis
git switch Luis_

Ya en mi rama personal, procedo a trabajar. Siguiendo un proceso similar al inicial:
- Realizamos un commit con _git commit -m “Añadido el botón y su funcionalidad en JS y CSS”_
- Actualizamos la rama main para que tenga los últimos cambios con _git pull origin main_
- Cambiamos a la rama main y traemos los cambios de la rama personal con _git switch main_ y _git merge Luis_


Para llevar a cabo el pull request, podemos hacerlo gráficamente desde GitHub o con comandos mediante Git.

En el primer caso, simplemente accedemos a la pagina de nuestro pull request y en el fondo encontraremos un botón verde que dice "Merge pull request".

Si preferimos hacerlo en Git, debemos seguir los siguientes pasos:
- Actualizar nuestro repositorio local con los últimos cambios: _git pull origin Luis_
- Cambiar a la rama del pull request: _git checkout Luis_
- Hacer un merge con el main: _git merge main_
- Hacer un push de los cambios: _git push -u origin Luis_
