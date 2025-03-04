README DE SERGIO BUZ EGIDO

PREPARACIÓN
 - Se han creado los repositorios inciales vacios para poder modicarlos.
 || mkdir ProyectoInicial ||
 || mkdir css ||
 || mkdir javascript ||
 || touch css/style.css ||
 || touch javascript/miijava.js ||
 - Realizado un commit
 || git innit . ||
 || git commit -am "Rama principal" ||
 - Creados los repositorios remotos den Github y subido el proyecto completo
 || git remote add origin *enlace* ||
 || git branch -M main ||
 || git push -u origin main ||


TRABAJO COLABORATIVO
 - Añadidos los colaboradores (Luis y Anais) a traves de settings/collaboratos
 - Creada una rama con mi nombre
  || git branch Sergio ||
 - Se ha añadido el CSS al documento mediante VSC
 - Subidos a mi rama los cambios realizados
  || git commit -am "Rama Sergio, Añadido el css" ||
  || git push ||

INTEGRACIÓN DEL PROYECTO
 - Realizado un pull request desde GitHub
 - Fusión de rama Sergio a rama Main
 || git merge Sergio ||

CONFLICTOS
 - Ya que mi rama ha sido la última en subirse, el archivo css estaba modificado ya con los cambios de Luis, por tanto, he tenido que hacer un merge manual, escogiendo con que quedarme y que borrar.
 - Al hacer el merge de mi rama al main se han borrado los readme de Luis y Anais. Me ha costado dios y ayuda que no se borraran pero al final revirtiendo el cambio con "git reset --hard 583e6d8" y subiendo los archivos de nuevo con "git push --set-upstream origin main --force" logré volver al Main con sus readme. Para fusionar mi rama sin borrar sus archivos hice una copia de sus readme en mi rama para que al hacer el merge, los README de main tuvieran un archivo sobre el cual volcarse y no se borraran
