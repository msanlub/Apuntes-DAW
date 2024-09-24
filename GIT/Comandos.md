## Principales comandos

```
git -v
git -h
git init
git branch -m main
git status
git add <file> 
git commit
git commit -m 
git push
git pull
git log
git checkout
git reflog
git diff
git tag nombre_etiqueta
git tag
```

- `git -v`-> versión de git
- `git -h`-> help
- `git init`-> inicia un proceso en git (se debe hacer en la carpeta raíz)
- `git branch -m main`-> cambiar el nombre de rama principal de proyecto
- `git status`-> para ver el estado de git, si se han hecho commit, si se ha modificado algún fichero...
- `git add <file> o .`-> añade el fichero o todos con el . y quedan preparados para el commit o fotografía. Se recomiendo hacer un git status antes para ver qué se está subiendo.
- `git commit`-> lanza una fotografía de los archivos
- `git commit -m`-> para poner un comentario a la fotografía
- `git push`-> sube los cambios a github
	- `git push origin main`
- `git pull` -> descarga los cambios de github
- `git log`-> para ver los commits, indica donde esta el HEAD o puntero
	Para verlo de una manera formateada por asi decirlo poner:
		`git log --graph
		`git log --graph --decorate --all --oneline --pretty=oneline
- `git checkout <id_commit>`-> para volver a ese commit y cambiar el HEAD o puntero, el id lo se con `git log`
- `git reflog`-> resumen de todo lo que hemos hecho
- `git diff`-> indica los cambios sin necesidad de hacer foto o commit
- `git tag nombre_etiqueta`-> crea una etiqueta con nombre identificativo en el punto donde estemos, es decir, donde está el HEAD o puntero.
- `git tag`-> muestra todas las etiquetas
	- `git checkout nombre_etiqueta`-> cambiamos el HEAD a ese punto



