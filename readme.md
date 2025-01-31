# Comandos Git

<img src="https://user-images.githubusercontent.com/77423877/212448635-0d5a1db3-1480-4910-baa8-971115cd06a4.png" width=550>

## Configuraciones
`git config --global user.name "[nombre]"`  
Establece el nombre asociado a los commits  
  
`git config --global user.email "[correo-electronico]"`  
Configura el email asociado a los commits  
  
`git config --list`  
Muestra la configuración actual  

## Comandos básicos
`git init`  
Inicializa un repositorio Git  
  
`git status`  
Muestra el estado de los archivos y cambios realizados  
  
`git add [archivo]`  
Agrega el archivo al área de staging  
  
`git add .` o `git add -A`  
Agrega todos los archivos modificados al área de staging  
  
`git commit -m "Mensaje del commit"`  
Guarda los cambios del área de staging en un nuevo commit  
    
`git log`  
Muestra el historial de commits  

## Diferencias entre archivos
`git diff`  
Muestra las diferencias entre archivos modificados  
  
`git diff --name-only`  
Muestra solo los nombres de archivos modificados  
  
`git diff [archivo]`  
Muestra diferencias en un archivo específico  

## Revertir cambios
`git reset [archivo]`  
Quita el archivo del área de staging  
  
`git reset --soft HEAD~1`  
Deshace el último commit manteniendo los cambios  
  
`git reset --hard HEAD~1`  
Elimina completamente el último commit y sus cambios

`git reset --soft [id-commit]` / `git reset --hard [id-commit]`  
Regresa al commit especificado, conservando (soft) o eliminando (hard) cambios  

## Branches
`git branch [nombre-branch]`  
Crea una nueva rama  
  
`git branch`  
Lista todas las ramas y muestra la actual  
  
`git checkout [nombre-branch]`  
Cambia a la rama especificada  
  
`git merge [nombre-branch]`  
Fusiona una rama con la rama actual  
  
`git branch -D [nombre-branch]`  
Elimina una rama localmente  
  
`git push [remoto] :[nombre-branch]`  
Elimina una rama en el repositorio remoto

## Repositorio remoto
`git remote add [remoto] [url]`  
Conecta el repositorio local con uno remoto  
  
`git remote` / `git remote -v`  
Muestra los repositorios remotos configurados  

`git remote rm [remoto]`  
Elimina la conexión con un repositorio remoto  
  
`git remote set-url [remoto] [nueva-url]`  
Actualiza la URL de un repositorio remoto  
  
`git push -u [remoto] [rama-local]`  
Primer push de una rama al repositorio remoto  
  
`git push`  
Envía cambios al repositorio remoto (pushes posteriores)  
  
`git pull [remoto] [rama]`  
Obtiene cambios del remoto y fusiona con local  
  
`git fetch`  
Descarga cambios del remoto sin fusionarlos  
  
`git clone [url]`  
Clona un repositorio remoto localmente  

## Libro gratuito de Git
[Pro Git (versión en español)](https://git-scm.com/book/es/v2)
