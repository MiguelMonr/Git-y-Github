## Git 

# Un poco de historia de git 

El desarrollo del kernel de Linux, iniciado por Linus Torvalds, originalmente usaba el sistema de control de versiones llamado BitKeeper. 
Sin embargo, en 2005, la relación entre la comunidad de desarrollo de Linux y la empresa detrás de BitKeeper se rompió. Linux requería un sistema de control de versiones que fuera:

Distribuido
Rápido
Con un diseño robusto
Capaz de manejar grandes proyectos como el kernel de Linux

En respuesta a esta necesidad, Torvalds aplico la de "si quieres que las cosas sean como quieres hazlas tu" y creo git en menos de 10 dias. 
Todo esto para poder gestionar el kernel de linux. 

## Y bueno, ¿qué es Git? 
Git es un sistema de control de versiones que permite rastrear los cambios que hemos hecho 
en un conjunto de archivos a traves de una linea de comandos (¿Qué significa esto? Que se maneja a traves de una terminal? \**\)

Git es un proyecto libre y open source* que funciona de manera distribuida; por lo que es fácil de escalar.  

> * Open source refiere a un tipo de software cuyo código fuente es accesible y libre para el público. Esto significa que cualquier persona puede ver, modificar y distribuir dicho software según lo estipulado por su licencia. 
La idea detrás del código abierto es promover la transparencia, la colaboración y la libre distribución de software.

> ** Si bien existen herramientas como git kraken o git desktop en este curso trabajaremos con git desde la terminal. 

Implentar git en nuestros proyectos permite: 
Crear flujos de trabajo al trabajar con más personas
Administrar proyectos
Rastrear cambios


# Conceptos de git
Al trabajar con git por primera vez nos encontramos con conceptos nuevos que pueden llegar a asustarnos un poco:  ¿qué es un repo?, ¿Mergear una rama?, ¿Qué es un commit?, ¿Matar el mapa después de haber forkeado al hijo?. Todos estos conceptos los desarrollaremos a continuacion: 

Repositorio: Un repositorio, a menudo abreviado como "repo", es un espacio digital donde se almacena y gestiona un proyecto. Puede contener código fuente, imágenes, documentos, y otros archivos. Es el corazón de cualquier proyecto en GitHub.


Commit: Registros de los cambios realizados en un proyecto. 


Branches: Linea independiente de desarrollo en el repositorio. 

>Stages de Git
1. **Working Directory**: Aquí haces lo cambios de tus archivos, no se actualizan hasta que los pongas en un commit.
2. **Staging Area**: En este caso se suben a un espacio temporal los cambios que preparas para un commit.
3. **Committed**: Cuando estas listo para subir los cambios que se agregaron  en el paso anterior. Se crea una grabación de los cambios con un mensaje para explicarlos.
4. **Remote Repository**: Con los comandos de `push` y de `pull` se actualiza el repositorio remoto o se descargan los cambios del repositorio remoto.

>Estados de un archivo en Git
## Estados de un Archivo en Git

1. **Modified (Modificado):** :
  - Los cambios en el archivo se han realizado pero aún no se han registrado en Git.
  - Se pueden deber a modificaciones en el contenido del archivo.

2. **Staged (Preparado):**
  - Los cambios han sido marcados para ser incluidos en el próximo commit.
  - Utilizando `git add`, se preparan los cambios para ser confirmados.

3. **Committed (Confirmado):**
  - Los cambios han sido registrados de manera permanente en el historial de Git.
  - Se utiliza `git commit` para confirmar los cambios previamente preparados.

# Terminal

Es una interfaz que nos permite interactuar con el sistema operativo mediante comandos de texto. Se podria decir que es una manera en la que nos comunicamos directamente con la computadora







