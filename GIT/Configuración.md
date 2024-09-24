
## Configuración de git: sistema de control de versiones

1. Descargar git (Enlace a página oficial)[https://git-scm.com/]  e instalar según SO.
2.  `git config --global user.name "marta"
3.  `git config --global user.email "msanchezl@iesrafaelalberti.es"
4.  Puedes configurar alias (crear un comando), por ejemplo:
		- `git config global alias.tree "log --graph --decorate --all --oneline"
		Cada vez que use `git tree` se verá una rama con esas características.
		-  `git config --global init.default Branch main`
		Cambia a la rama principal globalmente.