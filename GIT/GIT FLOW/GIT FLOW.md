
**Git Flow** es una metodología o flujo de trabajo en Git que organiza el proceso de desarrollo de software mediante una estructura clara de ramas (branches). Se basa en dos ramas principales de larga duración (`main` y `develop`) y utiliza ramas de soporte (`feature`, `release`, `hotfix`) para gestionar de manera eficiente el desarrollo de nuevas funcionalidades, lanzamientos y correcciones de errores.

### Estructura de ramas en Git Flow

1. **Rama principal (`main`)**:
    
    - Es la rama de producción.
    - Siempre está estable y lista para ser desplegada.
    - Sólo contiene versiones que ya han sido lanzadas o etiquetadas (tags).
2. **Rama de desarrollo (`develop`)**:
    
    - Aquí es donde se integran las nuevas funcionalidades que están listas para una próxima versión.
    - Se considera la base para el desarrollo continuo y es la rama de trabajo principal para los desarrolladores.
3. **Ramas de soporte**:
    
    - **`feature/`:** Para desarrollar nuevas funcionalidades o mejoras.
    - **`release/`:** Para preparar una nueva versión que se va a lanzar.
    - **`hotfix/`:** Para corregir errores críticos en producción.

## Instalación:

**En Linux**:

`sudo apt-get install git-flow`

## Inicialización
### Inicializar Git Flow en un proyecto

Una vez instalado Git Flow, puedes inicializarlo en tu repositorio:

`git flow init`
