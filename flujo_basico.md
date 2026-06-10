git status, git add, git commit.

Cuando trabajamos con git hay un flujo basico de 3 comandos para subir los cambios a la rama en la cual trabajamos. Estos comandos son, git status, git add y git commit

git status
Este comando sirve para ver el estado de los cambios realizados en la rama o en los archivos de la rama.
Los cambios que no estan traqueados, suelen ser archivos nuevos, se nos mostraran debajo de Untracked files en color rojo.
los cambios en archivos ya traqueados, se nos mostraran debajo de Changes not staged for commit.
Una vez que nosotros agregamos los cambios al staged, apareceran debajo de Changes to be committed en verde, esto nos indica que estan listos para hacer git commit.

git add
El comando git add, mueve los cambios registrados por git al staged. Si hacemos git add . se moveran todos los cambios al staged,
en cambio si hacemos git add nombre-archivo solo se moveran los cambios de ese archivo al staged.

git commit
Este comando guarda de forma permanente los cambios realizados. El commit contiene informacion como:
    - cambios
    - autor 
    - fecha 
    - mensaje 
    - referencia al commit anterior

Es importante tener en cuenta que los commits representan una idea logica del cambio.
Por lo que hay una convencion de como escribir los commits para que todo este ordenado y que transmita bien al resto del equipo el cambio realizado.
La manera correcta de escribir los commit es la siguiente. tipo(scope): descripción.
Tipos Principales 
    ● feat 
    ● fix 
    ● docs 
    ● style 
    ● refactor 
    ● test 
    ● chore
Ejemplos: 
    ● feat(user): agregar registro de usuario 
    ● fix(login): corregir error de sesión 
    ● docs(readme): actualizar instalación
