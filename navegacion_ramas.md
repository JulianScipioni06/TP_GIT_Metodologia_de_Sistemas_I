# git branch, git checkout y git switch

Decidimos agrupar estos tres comandos ya que los 3 comparten funcionalidad (navegar entre las ramas y crear ramas nuevas).

---

## git branch
se utiliza para crear, listar y eliminar ramas. 

* **`git branch`**: Muestra todas las ramas locales del repositorio y señala con un asterisco (`*`) en qué rama estamos trabajando actualmente.
* **`git branch nombre-de-la-rama`**: Crea una nueva rama.
* **`git branch -d nombre-de-la-rama`**: Elimina de forma segura una rama si ya fue fusionada con la principal. Usa `-D` (en mayúscula) para forzar la eliminación si es necesario.

## git checkout
Sirve para moverte entre las ramas y también para posicionarnos en commits viejos o anteriores al que estamos.

* **`git checkout nombre-rama`**: nos movemos a la rama seleccionada.
* **`git checkout -b nombre-rama`**: crea la rama llamada y nos mueve directamente.
* **`git checkout hash`**: mueve el puntero `HEAD` al commit con el hash seleccionado.

## git switch
Al igual que checkout, nos movemos entre las ramas, con la diferencia que switch lo tiene como función principal.

* **`git switch nombre rama`**: nos mueve a la rama.
* **`git -`**: nos regresa a la rama anterior en la que estábamos.
* **`git switch -c nueva-rama`**: crea una rama nueva.