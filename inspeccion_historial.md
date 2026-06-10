Inspeccion del historial GIT
En este apartado se detallan los comandos que nos permiten navegar por el historial del repositorio, chequear modificaciones,
en que momento se hicieron y quien las hizo.

Git Log
Este comando funciona como el cuaderno del proyecto.
Permite listar de forma cronologica todos los commits que se hicieron en la rama actual.
Ademas sirve para auditar la historia del repositorio, chequear los mensajes del commit, revisar los autores
y obtener los nombres necesarios para otras operaciones.
Algun ejemplo de uso podria ser: 'git log --online': esto lo que hace es compactar la informacion, lo que resulta en una
muestra de todos los commits en una sola linea.

Git Show
Mientras el git log nos da una vista general del historial, git show nos da una vista mas especifica del mismo.
Esto nos sirve para ver de forma detallada el contenido de un objeto, en general de un commit en particular. Si a este no
le pasamos ningun parametro, por defecto va a mostrar el ultimo commit hecho.
Este nos muestra el autor, la fecha, el diff detallado, que vendria a ser las lineas que se agregaron en verde o las que se 
eliminaron en rojo en los archivos correspondientes.
El ejemplo de uso es: git show <nombre_del_commit>

Git Diff
Este comando se usa para comparar distintas versiones de los archivos del proyecto.
Esto nos deja ver los cambios exactos que se hicieron en el codigo pero que todavia no fueron guardados definitivamente.
Algun ejemplo de uso o variante seria: 'git diff --staged': esto compara lo que agregamos al staged con el ultimo commit guardado, 
con esto revisamos detalladamente que es lo que va a entrar en el siguiente commit antes de ejecutarlo.
