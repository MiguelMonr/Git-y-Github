# Git-y-Github
En este repositorio se encuentra un curso introductorio a git y github. Se incluyen los stages de git así como distintos comandos basicos de terminal 

La presentación de este curso se encuentra en: https://www.canva.com/design/DAF8RfgU_Iw/6rDU_fDPMH4r-kcgt0cYWw/view?utm_content=DAF8RfgU_Iw&utm_campaign=designshare&utm_medium=link&utm_source=editor

# Importante
* Windows:
 Para los sistemas operativos windows usaremos wsl, es importante que lo tengas descargado https://learn.microsoft.com/es-es/windows/wsl/install
 Para instalar git en wsl usaremos `sudo apt update` y después `sudo apt install git` para tener listo su git.
 Descarguen en Visual Studio la extensión de wsl para poder usar los archivos de wsl en el Studio.


* MacOS:
  - Algunos equipos mac ya tienen git instalado por default, para saber si el tuyo lo tiene corre el siguiente comando en tu termial `git --version`
  - Si no tienes git entonces lo descargaremos con brew con `brew install git`
  - Aaaahora bien, si no tienes brew puedes con el siguiente comando desde tu terminal (puede tardar un poco) `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Hom...)"`

Después configuren su cuenta de git con los comandos `git config --global user.name "Nombre de Ususario"` y `git config --global user.email "correo electronico"`.

>Comandos basicos para que se puedan ayudar al usar git en la terminal:
1. `ls directorio/`: permite conocer los archivos dentro de un directorio.
2. `cd donde/queremos/ir`: permite movernos entre los directorios e ir a la carpeta en especifico a la cual queremos ir.
3. `mkdir nombre`: crea un directorio en el directorio en el que estamos.
4. `touch nombre`: crea un archivo en el directorio en el que estamos. 
5. `cp archivo donde/`: podemos hacer una copia de un archivo al directorio objetivo.
6. `cp -r directorio_a_copiar/ directorio_destino/`: con `-r` creamos una función recursiva que nos ayuda a copiar directorios y sus contenidos.
7. `nano archivo`: nos deja abrir un archivo y leer sus contenidos.
8. `rm archivo`: eliminamos un archivo.
9. `rm -r dir`: eliminamos un directorio y sus contenidos.
> Empecemos con Git
* `git clone <url-del-directorio>`: crea un repositorio local que es una copia del directorio 
* `git pull origin main`: obtenemos una actualización del repositorio remoto al repositorio local.
* `git branch nombre`: creas una nueva rama.
* `git checkout nombre`: cambias a la rama 'nombre'. Usualmente estas en automatico en la rama 'Main'. **NO HAGAS CAMBIOS EN LA RAMA MAIN**, salvo que ya sea un cambio definitivo (se hace normalmente el merge en el repositorio remoto).
* `git add archivo`: agregamos un cambio de un archivo al espacio temporal para alistarlo para el commit a la rama. **NUNCA NUNCA NUNCA HAGAN GIT ADD .** El añadir más de un archivo en un solo add puede subir archivos de administración de carpetas de un sistema operativo en especifico, esos archivos (usualmente DSS store) pueden romper la computadora de un usuario de otro sitema operativo.
* `git rm archivo`: agregamos la acción de eliminar un archivo al commit.
* `git commit -m 'Pon un mensaje'`: agregamos un commit al repositorio con todos los cambios que hemos ido agregando.
* `git push`: realizamos los cambios que se prepararon, se agregaron a un commit y se colocaron en el repositorio remoto.

> Notas para buena practica
* No hagan un add con multiples archivos, haganlos indivudualmente.
* Trabajen con una branch diferente al main.
* Cuando hagan un commit expliquen los cambios en el mensaje para que se pueda saber que cambios se realizaron.
* Mantengan actualizados sus repositorios locales para no generar incompatibilidades.

## NO HAGAN GIT ADD .

# Recursos Adicionales
# Para git y terminal
- Juego para aprender git: https://ohmygit.org/
- Juego para familiarizarse con los comandos de la terminal: https://overthewire.org/wargames/bandit/
- Tutorial 1 para git: https://www.youtube.com/watch?v=3GymExBkKjE&t=3835s 
- Tutorial 2 para git: https://youtu.be/mBYSUUnMt9M?si=WXXAa5Ld143pHwjc

# Para github
- Tutorial para hacer pull requests: https://github.com/skills/introduction-to-github
- Tutorial para solucionar conflictos: https://github.com/skills/resolve-merge-conflicts



