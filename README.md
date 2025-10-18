# ComandosGit
``

## Al iniciar un proyecto 
explicacion | comandos
------------- | -------------
iniciar git en una carpeta | `git init`  
agregar los archivos | `git add .`
commit  | `git commit -m "texto del commit"`
crear la rama main del proyecto | `git branch -M main`
subir los cambios a la rama  | `git push -u origin main`


## subir lo cambios a un proyecto ya iniciado 
explicacion | comandos
------------- | -------------
ver estado| `git status`  
agregar los cambios | `git add .`  
si solo se quiere agregar un archivo especifico | `git add src/App.jsx`
commit  | `git commit -m "texto del commit o de lo que se realizo"`
subir cambios | `git push origin nombre_de_la_rama`


## Ramas
explicacion | comandos
------------- | -------------
saber en que rama estoy| `git branch` 
crear rama | `git branch nombre_rama_nueva`  
cambiar de rama | `git checkout nombre_rama_nueva`
subir rama a github | `git push -u origin nombre_rama_nueva`
eliminar la rama | `git push origin --delete nombre_rama_nueva`













