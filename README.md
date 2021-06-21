# Analizando el nivel de seguridad del entorno de Android

## Comandos de preparacion

$ git --version // Sirve para conocer las versiones

$ git help // Sirve para mostrar como se usa un comando, por ejemplo: $ git help log

$ git status // Sirve para ver el estado de los archivos que fueron modificados o agregados

$ git log --all --decorate --oneline --graph

$ ssh-keygen -t rsa -C "lucianux@gmail.com"
// Sirve para generar una clave ssh para establecer una conexion segura.
// Pedirá un path para donde se va a guardar el archivo que contiene la clave (usamos la que viene por defecto -> presionar enter).
// Pedirá una contraseña (no la establecemos -> presionar enter para que salte al siguiente paso).
// Ahora dentro del sitio de GitHub en "Settings" > "SSH Keys" > "Add SSH key", debemos añadir el contenido del fichero id_rsa.pub generado en ~/.ssh/
// $ ssh git@github.com  ... Para probar si funciona, tendría que devolver algo como así: "Hi lucianux! You've successfully authenticated, but GitHub does not provide shell access."
// Si devuelve lo último mezclado o no con algunos errores, entonces la prueba fue exitosa

## Comandos para iniciar un nuevo proyecto

$ git clone git@github.com:lucianux/workspace.git

## Comandos de rutina

$ git add . // Agrega todos los archivo nuevos y modificados

$ git commit -m "comentario de commit" // Publica los cambios al repositorio local

$ git push // Publica los cambios al repositorio remoto

## Comandos útiles

$ git checkout HEAD -- file.txt // Descarta los cambios locales de un archivo

## Fuentes

* http://learn.github.com/p/intro.html
* http://www.adictosaltrabajo.com/tutoriales/tutoriales.php?pagina=githubFirstStepsUploadProject
* https://help.github.com/articles/generating-ssh-keys/
* https://www.atlassian.com/git/tutorials
