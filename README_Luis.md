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
