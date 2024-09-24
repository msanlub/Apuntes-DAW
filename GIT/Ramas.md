## Crear ramas y trabajar con ellas

```
git branch nombre_rama
git switch nombre_rama
git merge main
git branch -d nombre_rama
```

- `git branch nombre_rama`-> crea nueva rama pero el HEAD sigue en el main
- `git switch nombre_rama`-> cambia el HEAD a nueva rama y cambia a la rama. Se lleva el último commit y todo lo actualizado de la rama.
- `git merge main`-> vuelca el main en la nueva rama. 
	Si existen conflictos no nos permite hacer merge, me vuelvo al IDE y resuelvo los conflictos. Una vez resuelto hago add y commit y compruebo con status, así el main quedaría actualizado.
	Una vez haya terminado en esta rama, si quiero volcarlo al main, tendría que hacer el merge opuesto para volcar la info en el main. Desde main (`git switch main`) compruebo si hay conflictos (`git diff nombre_rama`) y vemos lo modificado. Finalmente hago el `git merge nombre_rama`.
- `git branch -d nombre_rama`-> eliminar ramas desde main (aunque siempre quedan los commits)
