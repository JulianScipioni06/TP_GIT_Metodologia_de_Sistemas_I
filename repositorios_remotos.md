# Repositorios remotos

## git remote

El comando `git remote` permite ver o administrar los repositorios remotos vinculados al proyecto.

### Comandos útiles:

* `git remote -v` → muestra los repositorios remotos y sus direcciones.
* `git remote add origin URL` → agrega un repositorio remoto.

---

## git push

El comando `git push` se utiliza para enviar nuestros commits al repositorio remoto.

### Comandos útiles:

* `git push origin main` → envía los cambios a la rama `main`.
* `git push -u origin nombre-rama` → envía la rama y la vincula con el repositorio remoto para futuros `push`.

---

## git pull

El comando `git pull` permite traer los cambios del repositorio remoto y actualizarlos en nuestra rama local.

### Comandos útiles:

* `git pull origin main` → descarga e integra los cambios de `main`.
* `git pull` → actualiza la rama actual desde el remoto configurado.

