# Comandos de terminal

### Introducción

**Bash** es una interfaz muy potente de línea de comandos, la cual es utilizada escribiendo comandos dentro de una terminal (como CMD en Windows). Este breve material pretende ayudarte a conocer acerca de los comandos mas utilizados y sus funciones.

> Su nombre es un [acrónimo](https://es.wikipedia.org/wiki/Acr%C3%B3nimo) de *Bourne-again shell* ("shell Bourne otra vez") haciendo un juego de palabras (*born-again* significa "[nacido de nuevo](https://es.wikipedia.org/wiki/Cristiano_renacido)") sobre la [Bourne shell](https://es.wikipedia.org/wiki/Bourne_shell) ([sh](https://es.wikipedia.org/wiki/Sh)), que fue uno de los primeros intérpretes importantes de Unix. («Bash», 2019)



### Comandos comunes

***mkdir: make directory***
Crea directorios (en Windows comúnmente llamados carpetas 😜).

***pwd: print working directory***
Muestra donde te encuentras en el sistema de archivos.

***cd: change directory***
Esta es la forma con la cual te mueves dentro del sistema de archivos.

> Existen dos directorios especiales que puedes utilizar con el comando **cd**:
>
> 1. `./` representa el directorio actual.
> 2. `../` representa el directorio inmediato superior al actual.
>    Cuando se ingresa la dirección donde esta ubicado un archivo se conoce como ruta (*PATH*).
> 3. `~` representa el directorio de inicio del usuario con una sesión iniciada.

***ls: list***
Imprime en pantalla todos los archivos y/o directorios existentes en el directorio actual.

***cp: copy***
Copia un archivo hacia otro archivo.

***mv: move***
Copia un archivo hacia un nuevo archivo ó ruta, y elimina el archivo original.

***rm: remove***
Elimina permanentemente el(los) archivo(s) proporcionado(s).

***rmdir: remove directory***
Elimina el directorio indicado. Este comando solo funciona con directorios vacíos.

***touch: remove directory***
Utilizado principalmente para cambiar la fecha y hora de última modificación de un archivo, pero si el archivo no existe este comando lo crea.



### Bibliografía

Bash. (2019). En *Wikipedia, la enciclopedia libre*. Recuperado de <https://es.wikipedia.org/w/index.php?title=Bash&oldid=113920024>

R. Clint Whaley. (s/f). *Introduction to Linux command line*. Recuperado de <http://homes.sice.indiana.edu/rcwhaley/teach/intromat/pdf/linux_intro.pdf>



# Práctica (Estructura de sitio web)

### Crear la siguiente estructura de directorios y archivos

```
Repositorio
├── 01-Practica
│   ├── node_modules
│   │   └── bulma
│   │       └── css
│   │           └── bulma.css
│   └── src
│       ├── css
│       │   └── styles.css
│       ├── images
│       │   └── logo.png
│       ├── js
│       │   └── app.js
│       ├── index.html
│       └── package.json
└── README.md

9 directorios, 7 archivos
```



### Pasos para realizar la estructura

```bash
# 1. Crear el directorio inicial
$ mkdir Repositorio

# 2. Ingresar al directorio recien creado
$ cd Repositorio

# 3. Crear el archivo README.md
$ touch README.md

# 4. Crear los directorios node_modules y src
$ mkdir node_modules src

# 5. Crear los directorios bulma/css dentro de node_modules
$ mkdir -p node_modules/bulma/css

# 6. Crear el archivo bulma.css dentro de node_modules/bulma/css
$ touch node_modules/bulma/css/bulma.css

# 7. Crear los archivos index.html y package.json dentro de src
$ touch src/index.html
$ touch src/package.json

# 8. Crear los directorios css, images y js dentro de src
$ mkdir src/css src/images src/js

# 9. Crear el archivo styles.css dentro de src/css
$ touch src/css/styles.css

# 10. Crear el archivo logo.png dentro de src/images
$ touch src/images/logo.png

# 11. Crear el archivo app.js dentro de src/js
$ touch src/js/app.js
```

