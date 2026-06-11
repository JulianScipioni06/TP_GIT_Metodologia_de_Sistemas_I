# Configuración del Entorno de Git

En este archivo se detalla los comandos fundamentales para verificar la instalación de Git, personalizar la identidad del usuario y comenzar a trabajar en un nuevo proyecto de forma local.

---

## Verificacion de la instalacion
   
### Git version:
Este comando se utiliza para comprobar que Git se encuentre instalado en el sistema y conocer la versión exacta con la que se esta trabajando.

* **Comandos:**
  `git --version`

---

## Git config
Este comando nos permite configurar y modificar los parametros de git, Como el nombre de usuario y el correo electronico que van asociados a los commits. 

* **Comandos:**
  `git config --list`: Nos muestra toda la configuracion de git.

* **-Global:** Afecta a todos los repositorios en los que participe el usuario
  `git config --global user.name "Nombre de usuario"`
  `git config --global user.email "tu_correo@gmail.com"`

* **-Local:** Solo afecta al repositorio actual.   
  `git config user.name "Nombre de usuario"`
  `git config user.email "tu_correo@gmail.com"`
