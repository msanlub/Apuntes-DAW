## Comandos para trabajar con git y GitHub

```
git remote add origin <direccion_repo>
git push
git fetch
git pull
git clone <direccion_repo>
git fork
git pull request
```

- ` git remote add origin <direccion_repo>` -> para asociar mi repo local a un repo creado en gitHub
- `git push`-> sube cambios al repo de github, antes hacer add y commit.
- `git fetch`-> se descarga el historial de cambios en mi local, sin hacerse los cambios
- `git pull`-> se descarga el historial de cambios y los cambios, suele haber conflictos. Si es el primer pull, antes se debe hacer un merge del main.
- `git clone <direccion_repo>`-> clonamos un repositorio nuevo en nuestro local, se copia la direccion desde el ssh
- `git fork`-> en el caso de no tener permisos en el repo, usamos fork para hacer una copia de un repo de otra persona y copiarmela a mi repo para poder modificarlo.
- `git pull request`-> después del fork y añadir mis cambios, se hace el pull al original. El propietario debe aceptar los cambios.