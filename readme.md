# ¿QUE ES GIT?

Git es un sistema de control de versiones que nos ayuda a guardar el historial de cambios y crecimiento de los archivos de nuestro proyecto mediante la colaboración mutua que nos hará la vida más fácil.

# PARA QUE SIRVE
* Aloja tu repositorio de código y te brinda herramientas muy útiles para el trabajo en equipo, dentro de un proyecto.
* Puedes contribuir a mejorar el software de los demás. 
* Provee de funcionalidades para hacer un fork y solicitar pulls.
* Vamos a poder trabajar en equipo de una manera muy sencilla y optimizada, de forma que si tenemos dos o tres personas trabajando en ciertas funcionalidades del proyecto y nosotros podemos estar trabajando en nuestra parte del código. Cuando acabamos de desarrollar nuestro código, utilizamos Git para mezclar los cambios con los otros compañeros, de forma que el código se mezcla de manera perfecta sin generar ningún tipo de fallo y de forma rápida.

# Estructura de trabajo de Git
![Estructura de git](http://blog.podrezo.com/wp-content/uploads/2014/09/git-operations.png)

# comandos para el uso de git

### COMANDOS BAISCOS
* **cat nombreArchivo** --(Sirve para)--> visualizar el contenido de un archivo.
* **pwd** --(Sirve para)-->  indica la ruta.


### CONFIGURACION DE USUARIO
* **git config -l**  --(Sirve para)--> permite ver toda la configuracion de usuario.
* **git config --list --show-origin** --(Sirve para)--> ver toda la configuracion de usuario(mas detallada).
* **git config --global user.name** --(Sirve para)--> configurar usuario.
* **git config --global user.email** --(Sirve para)--> configurar email.


### VISUALIZAR EL CONTENIDO EN EL REPOSITORIO
* **ls** --(Sirve para)--> enlista los archivos.
* **ls -al** --(Sirve para)--> enlista todos los archivos también  incluidos y en lista.
* **ls -a** --(Sirve para)--> muestra todos los archivos, pero no en lista.


### PARA PODER ENVIAR LOS CAMBIOAS AL REPOSITORIO LOCAL
* **git init** --(Sirve para)--> indica la carpeta Master.
* **git status** --(Sirve para)--> indica si ha habido algún cambio en los archivos y no se han añadido al repositorio.
* **git add .** --(Sirve para)--> envía  todos los documentos a la memoria RAM.
* **git commit -m "Mensaje"** --(Sirve para)--> envía  todos lo que este en la memoria ram a el repositorio local.

  *en caso de enviar un commit sin mensaje se abrira un editor de codigo(vim), para salir
  es (Esc+Shift+z+Z)

* **git rm** --(Sirve para)--> lo saca de la lista de archivos en la memoria ram.
* **git rm --cached** --(Sirve para)--> lo saca de la lista de archivos para el commit.
* **git show nombreArchivo** --(Sirve para)--> muestra los cambios que han ocurrido en el archivo que se ha especificado.
* **git show** --(Sirve para)--> muestra los cambios que han ocurrido en un archivo.
* **git diff** --(Sirve para)--> para comparar lo que tengo en staging(RAM) y el directorio de trabajo.
* **git diff versionA  versionB** --(Sirve para)--> comparar versiones.

## RAMAS

### CREACION DE RAMAS
* **git branch nombreRama** --(Sirve para)--> crea una rama
* **git checkout nombreRama** --(Sirve para)-->podemos cambiar entre ramas


#### FUSION DE RAMAS
1. Primero me coloco en la rama master
2. hago el  merge a la rama secundaria
* **git merge nombreRamaB** --(Sirve para)-->hace el merge


##  Como Recuerar Versiones.
* **git log** --(Sirve para)--> elista todas las versiones que existen(todos los commits).
    * --start //mas informacion.
* **git reset** --(Sirve para)--> nos permite volver a la version anterior.
* **git reset versionName --hard** --(Sirve para)--> Regresa todo a la version anterior y borra lo que este en RAM.
* **git reset version --soft** --(Sirve para)--> en el directorio de trabajo coloca la versiona anterior, pero no borra todo lo este en la Memoria RAM.
* **git checkout versionName nombreArchivo** --(Sirve para)--> trae el archivo en cierta version
    * git checkout master nombreArchivo.
* **git reset HEAD** --(Sirve para)--> Este es el comando para sacar archivos del área de Staging(RAM).


## Subir a GITHUB
* **git remote add origin rutaGithub** --(Sirve para)--> añadimos un repositorio remoto.
* **git push origin master** --(Sirve para)--> envía lo del directorio a github.
* **git pull origin master** --(Sirve para)--> trae los archivos de gitHub a el repositorio local.

 "cuando se va a fusionar los archivos saldrá un error porque las historias no coinciden, para forzar si fusión se usa".
* **git pull origin master --allow-unrelated-histories** --(Sirve para)--> fuerza la fusión de historias.
* **git remote** --(Sirve para)--> Te muestra origin
* **git remote -v** --(Sirve para)--> Te muestra las opciones que puedes hacer y el enlace de donde lo vas hacer
* **git config --get remote.origin.url** --(Sirve para)--> Retorna la url del repositorio remoto, desde tu repositorio local.



