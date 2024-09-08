## Github
Primero lo primero: git y github NO SON LO MISMO. Puede resultar un poco confuso a veces recordar cual es cual pero la gran diferencia es que
1) git es un sistema de control de versiones que esta instalado de manera local (que esta instalado en sus laps pues) mientras que github es una plataforma
2) que permite la colaboracion entre desarrolladores. En pocas palabras github usa git, no al reves.
3) git es mantenido por linux,por lo tanto es open source, y github por microsoft.

# Local y remoto
En la primera parte hablamos un poco de repositorios locales, pero ¿que significa esto? Github, como lo mencionamos, es un servicio de hosting. En el estan almacenados miles de repositorios en el que lxs desarroladorxs rastrean su trabajo. Cada uno de ellxs, si quiere, puede tener una version de ese repositorio en su equipo (o local) y hacer cambios. Sin embaaaargo, los cambios en el repo remoto (el que se encuentra en github)
no se van a ver reflejados en los locales a menos que ejecutemos ciertos comandos; la misma logica aplica con los locales, los cambios que hagamos en nuestros equipos no se veran reflejados hasta que querramos. 

# ¿Cómo se relacionan git y github? Claves SSH
Las claves ssh aparecen por primera vez en 1995 con el objetivo de proteger los datos entre dos maquinas. En github las utilizamos como un metodo de autenticación y conexión ya que es un protocolo bastante seguro. A traves de ellas podemos mandar nuestros cambios al repositorio remoto. Hay que resaltar que se generan en pares: una clave pública y una clave privada. La clave pública se comparte con el servidor remoto, mientras que la clave privada se guarda en secreto en el equipo del usuario. Cuando el usuario intenta iniciar sesión en el servidor, este utiliza la clave pública para cifrar un desafío. El usuario then debe descifrar el desafío con su clave privada. Si el descifrado es correcto, el usuario podrá iniciar sesión.
 ## IMPORTANTE: las ssh son vitales para conectar tu computadora con servicios en la nube. Por lo cual es de vital importancia que NO SE COMPARTAN. Gracias a ella, en el peor de los casos, un agente maligno puede acceder a toda la informacion de tu computadora. 

> Aquí el tutorial para configurarlas: https://docs.github.com/es/authentication/connecting-to-github-with-ssh/checking-for-existing-ssh-keys<

# Comandos de conexion
Para poder sincronizar nuestro cambios y mandarlos al repositorio remoto lo hacemos atraves de un par de comandos de git (siempre y cuando todos ellos ya hayan sido commiteados)
- `git push`: se utiliza para enviar los cambios locales al repositorio remoto. Es decir, actualiza el repositorio remoto con los cambios que has realizado en tu copia local.

¿Qué pasa si se hacen cambios en el remoto?, ¿Se pueden traer a nuestro local? Sí se puede, con los siguientes comandos: 

- `git fetch`: Este comando se utiliza para obtener los cambios del repositorio remoto sin fusionarlos con tu copia local. Es decir, descarga los cambios del repositorio remoto, pero no los aplica a tu copia local.
- `git pull`: Este comando se utiliza para obtener los cambios del repositorio remoto y fusionarlos con tu copia local. Es decir, actualiza tu copia local con los cambios que se han realizado en el repositorio remoto.

# Cuidado
Al empezar a trabajar con repositorios locales y remotos junto con nuestro equipo si no existe la comunicación adecuada puede que una o más personas trabajen sobre el mismo archivo;
tal vez alguien borre un archivo y otro este trabajano en el. O peor aun, ¡varias personas estan trabajando sobre la rama principal! Si pasa alguna de estas situaciones lo más probable es que ocurra un conflicto.

# Conflictos 
Los conflictos en Git ocurren cuando se fusionan dos ramas que tienen cambios en los mismos archivos. Cuando esto sucede, Git no puede determinar automáticamente qué cambios se deben conservar y cuáles se deben descartar. En este caso, se produce un conflicto de fusión y el usuario debe resolverlo manualmente.

Tipos de conflictos:

- Conflictos de fusión: Se producen cuando dos ramas modifican las mismas líneas de un archivo. Git no puede fusionar automáticamente estos cambios, por lo que debes resolverlos manualmente.
- Conflictos de eliminación: Se producen cuando una rama elimina un archivo que ha sido modificado en otra rama. Git no puede fusionar estos cambios, por lo que debes decidir qué versión del archivo deseas conservar.
- Conflictos de cambio de nombre: Se producen cuando un archivo se renombra en una rama y se modifica en otra rama. Git no puede fusionar estos cambios automáticamente, por lo que debes decidir qué nombre y contenido del archivo deseas conservar.

Ahooora bien. Tener conflictos no implica que se acabe el mundo o que tu codigo ya no vaya a servir, tranquilx. Para poder solucionarlos existen varias tecnicas que nos pueden ayudar a solucionarlos. Si bien se pueden hacer desde git con comandos como git rebase o git cherry picking en este curso utilizaremos los pull request. 

Pull request: mecanismo formal dentro del control de versiones con Git para proponer cambios de código a un repositorio principal, ya sea un proyecto personal o colaborativo. Se trata de una solicitud que un desarrollador realiza para que sus modificaciones sean revisadas e integradas al código base ("mainline").

Issues: permiten a los desarrolladores y equipos gestionar tareas, hacer seguimiento de errores, discutir ideas y llevar un registro de mejoras dentro de un proyecto. Funcionan como un sistema de gestión de tareas o un sistema de tickets dentro de un repositorio.

