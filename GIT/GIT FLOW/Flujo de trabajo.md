### Flujo de trabajo con Git Flow


### Resumen del flujo de trabajo con Git Flow

1. **Ramas principales**:
    
    - `main`: contiene el código estable y lanzado.
    - `develop`: contiene el código en desarrollo.
2. **Ramas de soporte**:
    
    - **Feature**: se usa para desarrollar nuevas funcionalidades.
    - **Release**: se usa para preparar una nueva versión.
    - **Hotfix**: se usa para corregir errores críticos en producción.

## Desarrollo
#### 1. Desarrollar una nueva funcionalidad (rama `feature`)

Cuando deseas desarrollar una nueva funcionalidad, primero creas una rama `feature` que se basa en `develop`. Todo el trabajo relacionado con esa funcionalidad se hace en esa rama. Una vez completada, se integra de vuelta en `develop`.

**Ejemplo:**

1. Crear una nueva rama `feature`:
    
    bash
    
    Copiar código
    
    `git flow feature start mi-nueva-funcionalidad`
    
    Esto crea una rama `feature/mi-nueva-funcionalidad` basada en `develop`.
    
2. Desarrollas la funcionalidad en la nueva rama:
    
    bash
    
    Copiar código
    
    `git add . git commit -m "Añadir nueva funcionalidad"`
    
3. Cuando terminas la funcionalidad, cierras la rama:
    
    bash
    
    Copiar código
    
    `git flow feature finish mi-nueva-funcionalidad`
    
    Este comando:
    
    - Fusiona la rama `feature/mi-nueva-funcionalidad` de nuevo en `develop`.
    - Elimina la rama `feature/mi-nueva-funcionalidad` localmente y en el servidor remoto.

#### 2. Preparar una versión (rama `release`)

Cuando tienes varias funcionalidades listas en `develop` y deseas lanzar una nueva versión, creas una rama `release`. Aquí haces pruebas finales, ajustes menores y te preparas para lanzar.

**Ejemplo:**

1. Crear una nueva rama `release`:
    
    bash
    
    Copiar código
    
    `git flow release start 1.0.0`
    
    Esto crea una rama `release/1.0.0` basada en `develop`, donde "1.0.0" es el número de la nueva versión.
    
2. Realizas pruebas y ajustes finales en esta rama, y luego cuando todo está listo, la finalizas:
    
    bash
    
    Copiar código
    
    `git flow release finish 1.0.0`
    
    Este comando:
    
    - Fusiona `release/1.0.0` en `main`.
    - Fusiona también en `develop` (en caso de que haya correcciones hechas durante la fase de pruebas).
    - Crea una etiqueta (`tag`) en `main` para marcar la versión (`1.0.0`).
    - Elimina la rama `release/1.0.0`.

#### 3. Corregir errores críticos (rama `hotfix`)

Si surge un problema grave en producción, creas una rama `hotfix` a partir de `main` para corregir el error. Esta es la única situación donde trabajas directamente desde `main`.

**Ejemplo:**

1. Crear una nueva rama `hotfix`:
    
    bash
    
    Copiar código
    
    `git flow hotfix start 1.0.1`
    
    Esto crea una rama `hotfix/1.0.1` desde `main`, donde "1.0.1" es el número de la corrección.
    
2. Haces la corrección del error:
    
    bash
    
    Copiar código
    
    `git add . git commit -m "Corregir error crítico"`
    
3. Finalizas el `hotfix`:
    
    bash
    
    Copiar código
    
    `git flow hotfix finish 1.0.1`
    
    Este comando:
    
    - Fusiona la rama `hotfix/1.0.1` en `main`.
    - Fusiona también en `develop` (para asegurarse de que la corrección esté en el ciclo de desarrollo continuo).
    - Crea una etiqueta (`tag`) para la versión corregida (`1.0.1`).
    - Elimina la rama `hotfix/1.0.1`.

