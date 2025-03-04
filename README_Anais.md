# HTML
*Anais Carreño Monniot*

En esta prueba se trabajó en una rama que despues se fusionó, 
El html es de un ejemplo de formulario.

## Inicio del proyecto
  Para comenzar hubo que descargarse el proyecto inicial para poder empezar a trabajar en él.
    - `git clone URL ` 
    - Crear una rama  -> `git branch Anais`  // `git checkout -b Anais` (crea la rama y cambia automaticamente a ella)
    - Cambiar a la rama  -> `git checkout Anais`
    - Mostrar las ramas remotas  -> `git checkout -r`

  Desde ahi trabajar en las modificaciones del html y subirlas al repositorio
    - `git add .`
    - `git commit`
    - Fusionar mi rama al repositorio  -> `git merge origin/Anais`
    - Subir los cambios agitHub  -> `git push`

## Gestion y solución de conflictos
    Al modificar archivos ya sean propios o de un compañero si se hace en local habrá que revisar los cambios para comprobar 
    que no se han realizado cambios de manera accidental. Esto se realizará mediante los pull request. En cada commit y pull
    request se puede añadir un mensaje facilitando a los compañeros la revision de los cambios realizados.

    A la hora de revisar los pull request aparecen las siguientes opciones 
      ### Create a merge commit     
        Fusiona la rama con un commit extra que registra la unión de ambas.
        Mantiene el historial de commits de la rama fusionada.
        Uso: Si qse queire un historial detallado y ver exactamente qué commits se hicieron antes de la fusión.
            - `git merge Anais`
            
      ### Squash and merge
        Qué hace:
        Une todos los commits de la rama en uno solo antes de fusionarlo.
        No mantiene el historial de commits individuales, solo deja un único commit con todos los cambios.
        Uso:  Si la rama tiene muchos commits pequeños que no aportan mucho o si se quiere un historial más limpio y resumido.
          - `git merge --Anais`
          - `git commit -m "Descripcion"`
          
      ### Rebase and merge
      Mueve los commits de la rama a la punta de la rama destino, como si hubieran sido hechos directamente ahí.
      No crea un commit de merge, mantiene el historial lineal.
      Uso:   Si quieres un historial más limpio sin commits de merge.
            Si la rama tiene cambios que deberían integrarse como si siempre hubieran estado en la rama principal.
          - `git rebase Anais`

  Si se hiciesen los cambios desde gitHub no habria que revisar estos cambios ya que se ejecutarian directamente en el main.
      
