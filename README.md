# 💻 Guía  de Comandos Git y GitHub
---

## 1. Configuración Inicial
*Se ejecuta una sola vez al instalar Git en tu computadora para identificar quién hace los cambios.*

Explicación | Comando
------------- | -------------
Configurar tu nombre de usuario | `git config --global user.name "Tu Nombre"`
Configurar tu correo vinculado a GitHub | `git config --global user.email "tu@email.com"`
Ver tu configuración actual | `git config --list`

---

## 2. Iniciar un proyecto desde cero
*Cuando tienes una carpeta local nueva y quieres conectarla a un repositorio vacío en GitHub.*

Explicación | Comando
------------- | -------------
Iniciar git en la carpeta | `git init`  
Agregar todos los archivos | `git add .`
Crear el primer commit | `git commit -m "commit inicial"`
Crear o renombrar la rama principal a main | `git branch -M main`
Vincular tu carpeta con el repo de GitHub | `git remote add origin URL_DEL_REPOSITORIO`
Subir los cambios a la rama principal por primera vez | `git push -u origin main`

---

## 3. Trabajo diario (Ciclo básico)
*El flujo normal de trabajo cuando estás programando y guardando tu progreso.*

Explicación | Comando
------------- | -------------
Ver el estado de tus archivos (modificados, agregados) | `git status`  
Agregar todos los cambios | `git add .`  
Agregar solo un archivo o carpeta específica | `git add src/App.jsx`
Crear un commit con los cambios | `git commit -m "texto de lo que se realizó"`
Subir los cambios a GitHub | `git push origin nombre_de_la_rama`

---

## 4. Ramas (Branches)
*Esenciales para no romper el código principal al agregar nuevas funciones o probar ideas.*

Explicación | Comando
------------- | -------------
Saber en qué rama estoy parado | `git branch` 
Crear una rama nueva | `git branch nombre_rama_nueva`  
Cambiar a una rama existente | `git checkout nombre_rama_nueva`
Crear una rama y cambiarte a ella de inmediato | `git checkout -b nombre_rama_nueva`
Subir una rama nueva a GitHub | `git push -u origin nombre_rama_nueva`
Eliminar una rama localmente | `git branch -d nombre_rama_nueva`
Eliminar una rama remota (en GitHub) | `git push origin --delete nombre_rama_nueva`
Fusionar otra rama hacia la que estás parado | `git merge nombre_de_la_otra_rama`

---

## 5. Colaboración y Sincronización
*Para trabajar en el proyecto de otra persona (tras hacer un Fork) o actualizar tu código.*

Explicación | Comando
------------- | -------------
Descargar un repositorio de GitHub a tu PC | `git clone URL_DEL_REPOSITORIO`
Descargar y aplicar los últimos cambios de GitHub a tu PC | `git pull origin main`
Traer información de ramas nuevas sin modificar tu código | `git fetch origin`
Ver qué repositorios remotos están conectados | `git remote -v`

> **💡 Nota sobre Pull Requests (PR):** Los Pull Requests se gestionan desde la interfaz web de GitHub. Una vez que subes tu rama (`git push origin tu_rama`), ve a la página del repositorio y haz clic en **"Compare & pull request"**.

---

## 6. Historial y Emergencias
*Para revisar el pasado del proyecto o solucionar errores antes de subirlos.*

Explicación | Comando
------------- | -------------
Ver el historial de commits | `git log`
Ver el historial resumido (un commit por línea) | `git log --oneline`
Deshacer cambios de un archivo antes de hacer commit | `git checkout -- nombre_del_archivo`
Deshacer el último commit (manteniendo los archivos modificados) | `git reset --soft HEAD~1`
**PELIGRO:** Borrar todos los cambios locales no guardados en un commit | `git reset --hard HEAD`













