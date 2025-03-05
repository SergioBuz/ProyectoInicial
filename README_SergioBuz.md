# README - Sergio Buz Egido

## 📌 Preparación

1. Se han creado los repositorios iniciales vacíos para poder modificarlos:
   ```sh
   mkdir ProyectoInicial
   mkdir css
   mkdir javascript
   touch css/style.css
   touch javascript/miijava.js
   ```
2. Realizado un commit inicial:
   ```sh
   git init
   git commit -am "Rama principal"
   ```
3. Creación y subida del repositorio remoto en GitHub:
   ```sh
   git remote add origin <enlace>
   git branch -M main
   git push -u origin main
   ```

---

## 🤝 Trabajo Colaborativo

1. Se han añadido los colaboradores (Luis y Anais) a través de:
   - *Settings > Collaborators*
2. Creación de una nueva rama con mi nombre:
   ```sh
   git branch Sergio
   ```
3. Se ha añadido el CSS al proyecto mediante Visual Studio Code.
4. Subida de los cambios a mi rama:
   ```sh
   git commit -am "Rama Sergio, Añadido el CSS"
   git push
   ```

---

## 🔄 Integración del Proyecto

1. Se ha realizado un *Pull Request* desde GitHub.
2. Fusión de la rama `Sergio` a la rama `main`:
   ```sh
   git merge Sergio
   ```

---

## ⚠️ Resolución de Conflictos

- Al ser mi rama la última en subirse, el archivo `style.css` ya había sido modificado por Luis, lo que generó un conflicto.
- Se realizó un *merge* manual, escogiendo qué cambios conservar y cuáles descartar.
- Al hacer el merge, los README de Luis y Anais fueron eliminados accidentalmente.
- Para solucionar este problema:
  1. Se revirtió el cambio con:
     ```sh
     git reset --hard 583e6d8
     ```
  2. Se subieron nuevamente los archivos con:
     ```sh
     git push --set-upstream origin main --force
     ```
  3. Para evitar la eliminación de los README de mis compañeros, hice una copia de sus archivos en mi rama antes de hacer el *merge*, asegurando que existieran en `main` durante la fusión.

---
