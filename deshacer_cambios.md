# Deshacer cambios GIT 

Git ofrece herramientas muy buenas para corregir errores o volver para atras.
El como se hara para deshacer los cambios depende de en que estado se encuentra la modificacion, 
es decir si esta en el directorio de trabajo, en el stage o ya guardada en un commit.

---

## 1.Git Restore

* Este comando nos facilita la opcion para recuperar archivos en nuestro espacio de trabajo local de forma segura.
Ademas de descartar modificaciones locales o deshacer un proceso de preparacion que todavia no fue guardado en un commit.
**Algun ejemplo de uso seria: 'git restore --staged <archivo>'**: lo que pasa aca es que saca el archivo del stage y lo manda devuelta
al directorio de trabajo. 



## 2.Git Reset
* Este comando nos permite mover el puntero de la rama actual en la que estas hacia un commit anterior en el historial.
Esto nos sirve para deshacer commits enteros de forma local si queremos por ejemplo reorganizar el trabajo.
**Un ejemplo de uso seria: 'git reset --soft <nombre>'**: esto deshace los commits siguientes al nombre indicado, pero a la vez 
conserva los cambios en el stage para que estos sean commiteados, por lo que no se pierde el codigo.

---

## 3.Git Revert 
* Este comando a diferencia del reset, es una via segura y profesional de deshacer cambios que ya fueron subidos
a un servidor remoto compartido.
Esto lo que hace es que en vez de borrar commits pasados y alterar la historia, crea un nuevo commit que hace lo inverso al 
commit que queremos borrar o anular, por lo que si en el commit original lo que queremos es agregar una linea de codigo, el revert
la elimina.
Es conveniente usarla en equipo, ya que al no alterar el historial, no genera conflictos ni rompe los repositorios locales de 
los demas integrantes.

  **El ejemplo de uso basico es:** **'git revert <nombre_del_commit>'**
