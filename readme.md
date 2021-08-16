# Aprende a usar un control de versiones más rápido que hacer un café:

## Contenido:

* ¿Qué es un sistema de control de versiones?
* Consejos antes de iniciar.
* ¿Cómo instalar Git?
* Comandos básicos en consola.

## ¿Qué es un control de versiones?

Enfocandolo al mundo de la programación, los sistemas de control de versiones son herramientas que ayudan a gestionar los cambios en un archivo o código fuente a lo largo del tiempo. Estas herramientas nos permiten tener un orden de los cambios realizados.
¿Te ha pasado que tienes muchisimas versiones de un proyecto o trabajo? Es probable que almenos 1 vez ocurrió por miedo a no perder el avance cuando algo estaba bien, funcionaba o simplemente era otra alternativa. Un controlador de versiones permite hacer eso sin tener que hacer decenas de copias del mismo proyecto y además puede llegar a fusionar los cambios que existen entre una versión y otra.

### Evita hacer esto usando un sistema de control de versiones:

<img src="https://miro.medium.com/max/1200/0*vjveQSD3TKHoqHc6.jpg" /> [imagen de: medium.com]

## Sistema de control de versiones - GIT

Es un sistema de control de versiones de código abierto y usado por millones de personas a lo largo de mundo, en este caso veremos como usarlo de forma local y en GitHub para tenerlo en la web, además veremos como trabajar de forma individual y coolaborativa.

## Consejos antes aprender GIT:

* Contar con una computadora.
* Crear una cuenta en [GitHub](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) (Opcional) pero si quieres exponer tus proyectos o trabajar de forma coolaborativa te aconsejo hacerlo.
* Tener un correo electrónico **tuyo** y que no olvidarás porque los cambios que hagas en los archivos serán firmados con información de ese correo (Posteriormente puede cambiarse el correo, pero es aconsejable establecer uno).


# ¡Empecemos!


## ¿Cómo empezar a usar Git?

Dirigete al sitio oficial de Git presionando [aquí](https://git-scm.com/), te desplegará una página como la siguiente:

<img src="media/oficialGit.png" style="border-radius: 5%;"/>

Dirigete al monitor que aparece a la derecha y presiona en "Download for" en este caso es un SO Windows, sin embargo, el sitio web sabrá  que sistema operativo tienes. 

<img src="media/download.png" style="border-radius: 5%;"/>

Comienzará a descargarse el instalador, sólo espera un momento a que finalice este proceso.

O bien, si necesitas alguna otra versión de git presiona en donde dice "Downloads" en la barra lateral izquierda y selecciona la que mejor se ajuste a las caracteristicas de tu sistema operativo.

<img src="media/version.png" style="border-radius: 5%;"/>

## Instalando Git:

Una vez que haya finalizado la descarga podremos instalar git en nuestro equipo. Da doble click sobre el elemento que se descargó, esa acción te desplegará una ventana como la siguiente:

<img src="media/instalacion/1.PNG" style="border-radius: 5%;"/>

Lee los *terminos y condiciones*
 del uso de *git* y presiona en **siguiente**, esto te mostrará lo siguiente:

<img src="media/instalacion/2.PNG" style="border-radius: 5%;"/>

Te recomiendo dejar las opciones seleccionadas por defecto. Presiona **siguiente** para seguir con el proceso de instalación.

<img src="media/instalacion/3.PNG" style="border-radius: 5%;"/>

Verás la siguiente ventana donde te pregunta el editor de código que usarás con git. Si aún no sabes que editor usarás, te recomiendo que dejes seleccionado **Vim**, esto no significa que siempre trabajarás con Vim, sino que sólo será el editor por defecto, más adelante podrás usar git en cualquier otro editor.
Presiona **siguiente**

<img src="media/instalacion/4.PNG" style="border-radius: 5%;"/>

Te recomiento que en este apartado presiones la opción de abajo y coloques **main** este nombre será el que adopte la rama principal de trabajo. (este nombre es libre de jerarquias y clasismos con respecto a master). Presiona **Siguiente**.

<img src="media/instalacion/5.PNG" style="border-radius: 5%;"/>

Mantén seleccionada la tercera opción para que puedas hacer uso de Git mediante cualquier otra terminal y no sólo desde la Git Bash que nos generará al final de esta instalación. Presiona **siguiente**.

<img src="media/instalacion/6.PNG" style="border-radius: 5%;"/>

Te recomiendo dejar la opción por defecto y dar **siguiente** en las proximas 6 ventanas.

<img src="media/instalacion/7.PNG" style="border-radius: 5%;"/>

En la ultima ventana sólo presiona **instalar** y espera a que este proceso termine.

### ¡Felicidades! Ya instalaste Git.

## <strong> Comandos básicos en consola </strong>

| Comando | Acción |
| --- | --- |
| `cd nombreCarpeta` | Se posiciona dentro de la carpeta con el nombre especificado |
| `cd ..` | Retrocede a una carpeta anterior de la que se está posicionada |
| `mkdir nombreCarpeta` | Crea una carpeta con el nombre indicado |
| `ls` (SO basado en Linux) | Lista todos los elementos que se encuentran en esa carpeta o directorio |
| `dir` (SO basado en Windows) | Lista todos los elementos que se encuentran en esa carpeta o directorio |

## <strong> Comandos básicos en Git </strong>

| Comando | Acción |
| --- | --- |
| `git --version` | Permite conocer la versión de git en el equipo |
| `git config --global user.name "Tu nombre"` | Permite establecer el nombre que queremos en git |
| `git config --global user.name "Tu nombre"` | Permite establecer el un nombre en git|
| `git config --global user.username "Tu nombre"` | Establece el nombre de username (Aquí colocarás el mismo nombre de usuario que colocaste al crear tu cuenta en GitHub) |
| `git config --global user.email "tuemail@example.com""` | Permite establecer el correo electrónico en la configuración de git (Si creaste tu cuenta en GitHub coloca el correo con el que creaste la cuenta) |
| `git init` | Permite inicializar git en esa carpeta |
| `git status` | Lista archivos nuevos, modificados o que no han sido relacionados aún a git |
| `git add nombreArchivo` | Agrega ese archivo al sistema de control de versiones git. Al hacerlo, git habrá referenciado los nuevos cambios |
| `git add .` | Agrega esos archivos al sistema de control de versiones git. Al hacerlo, git habrá referenciado los nuevos cambios |
| `git diff` | Nos muestra los cambios que hubo al agregar el archivo modificado. Muestra las modificaciones |
| `git commit -m "descripción"` | Git guarda los cambios hechos hasta ese momento (imaginatelo como guardar la partida en un videojuego) donde dice descripcion deberás describir la funcionalidad de los nuevos cambios, preferentemente no mayor a 50. caracteres|
| `git log` | Lista todos los commits hechos hasta la fecha|
| `git remote add origin EnlaceURL"` | Conecta nuestro repositorio local con uno externo, en este caso puede ser el enlace a un repositorio en GitHub.|
| `git remote -v` | Sirve para obtener información sobre la conexión que tiene el repositorio, normalmente se usa para verificar que está conectado correctamente.|
| `git push origin main/master` | Permite enviar los cambios del repositorio local al repositorio en GitHub, colocarás **main** ó **master** según el nombre que le hayas puesto en la instalación.|
| `git push origin nombreRama` | Permite enviar los cambios del repositorio local al repositorio en GitHub sobre la rama de ese nombre.|

## Trabaja con Git de forma Local:

* Crea una carpeta sobre la que estarás trabajando (sólo si apenas trabajaras un nuevo proyecto, sino sólo ve al paso que siguente).
* Posicionate en la carpeta trabajo mediante GitBash.
```
cd nombre_Carpeta
```
* Inicializa un repositorio con el comando `git init`.

```
$ git init
```

* Ejecuta el comando `git status` cada que hagas un cambio o añadas un nuevo archivos, este comando te listará los archivos que cumplan con ello. Si no tienes ningún archivo o aún no haces cambios te mostrará un mensaje como el siguiente: 

```
On branch main
nothing to commit, working tree clean
```

* Si tienes archivos listados en `git status` entonces ejecuta `git add nombreArchivo` ó `git add .` para agregar todos los archivos con modificaciones.

```
git add nombreArchivo

ó

git add .
```

* Realiza un guardado de tus cambios con un commit. Los commit llevan una breve descripción de lo que se hizo, por ejemplo: "Se corrigió un bug en...", "Se incorporó un menú", etc.

```
git commit -m "Descripción breve del funcionamiento"
```

* Si quieres ver los commit's que has hecho entonces usa `git log` que listará los commits realizados en ese repositorio.

```
git commit -m "Descripción breve del funcionamiento"
```

### ¡Con los pasos anteriores ya puedes trabajar de forma local sin problema!

## <strong>¿Cómo trabajar con Git & GitHub?</strong>

Para ello deberás tener una cuenta creada, si aún no la has creado presiona [aquí](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home).

* Dirigete al menú de GitHub e identifica el botón "new repository" o un equivalente, acontinuación te verás una imagen ilustrativa al respecto:

<img src="media/repo/new.png"/>

* Una vez que hayas presionado ahí te redigirá a la siguiente pantalla:

<img src="media/repo/name.png" style="border-radius: 5%;"/>

Aquí pondrás el nombre que quieres que tenga tu repositorio, puedes poner una ligera descripción acerca de lo que trata, poner la visibilidad pública o privada y decidir si agregar algunos archivos importantes como: `readme`(donde explicas a detalle tu proyecto), `gitignore`(indica los archivos que no subirá al repositorio) y `license`(Es el archivo que explica todos los terminos y condiciones al usar un proyecto).

* Llena el repositorio a tu gusto, en mi caso sólo puse lo siguiente:

<img src="media/repo/example.png" style="border-radius: 2%;"/>

Presiona en **Crear repositorio**

* En esta ventana verás información interesante, que nos permitirá conectar un repositorio de GitHub con uno local, en este tutorial tomaremos la segunda sección que dice "…or push an existing repository from the command line" y copiaremos la primer línea de comandos (Asegurare de tener en la parte de arriba seleccionada la opción HTTPS como se ve en la imagen):

```
git remote add origin https://github.com/YanniMartinez/Aprende-Git-en-5-Minutos.git
```

<img src="media/repo/conection.png" style="border-radius: 2%;"/>

* Repite los pasos de la sección anterior llamada "Trabaja de forma local con Git" o en ese mismo repositorio haz lo siguiente:

<img src="media/repo/gitRemote.PNG" style="border-radius: 2%;"/>

* Para verificar que se realizó correctamente la conexión ejecuta `git remote -v`

<img src="media/repo/remoteV.PNG" style="border-radius: 2%;"/>

* Si te listó 2 elementos ¡lo hiciste bien!

* Ahora sólo nos falta enviar los cambios locales al repositorio en GitHub, para ello ejecutamos el comando `git push origin main` ó `git push origin master` según como hayas configurado la instalación (en mi caso será `main`). Si es la primera vez que usas Git con GitHub te pedirá iniciar sesión para comprobar que eres tú el dueño de la cuenta (Si te da error verifica que hayas colocado nombre de usuario y correo al configurar tu Git, esto puedes consultarlo en los primeros pasos del manual).

<img src="media/repo/pushMain.PNG" style="border-radius: 2%;"/>

### Actualiza el sitio web de GitHub y ¡listo! Ya enviaste los archivos de un sitio local a tu GitHub.