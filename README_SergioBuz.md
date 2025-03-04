README DE SERGIO BUZ EGIDO

PREPARACIÓN
 - Se han creado los repositorios inciales vacios para poder modicarlos.
  (mkdir ProyectoInicial)
  _mkdir css_
  _mkdir javascript_
  _touch css/style.css_
  _touch javascript/miijava.js_ 
 - Realizado un commit
  _git innit ._
  _git commit -am "Rama principal"_
 - Creados los repositorios remotos den Github y subido el proyecto completo
  _git remote add origin *enlace*_ 
  _git branch -M main_ 
  _git push -u origin main_ 


TRABAJO COLABORATIVO
 - Añadidos los colaboradores (Luis y Anais) a traves de settings/collaboratos
 - Creada una rama con mi nombre
  _git branch Sergio_ 
 - Se ha añadido el CSS al documento mediante VSC
 - Subidos a mi rama los cambios realizados
  _git commit -am "Rama Sergio, Añadido el css"_ 
  _git push_ 

INTEGRACIÓN DEL PROYECTO
 - Realizado un pull request desde GitHub
 - Fusión de rama Sergio a rama Main
  _git merge Sergio_ 

CONFLICTOS
 - Ya que mi rama ha sido la última en subirse, el archivo css estaba modificado ya con los cambios de Luis, por tanto, he tenido que hacer un merge manual, escogiendo con que quedarme y que borrar.
 - Al hacer el merge de mi rama al main se han borrado los readme de Luis y Anais. Me ha costado dios y ayuda que no se borraran pero al final revirtiendo el cambio con "git reset --hard 583e6d8" y subiendo los archivos de nuevo con "git push --set-upstream origin main --force" logré volver al Main con sus readme. Para fusionar mi rama sin borrar sus archivos hice una copia de sus readme en mi rama para que al hacer el merge, los README de main tuvieran un archivo sobre el cual volcarse y no se borraran
