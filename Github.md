## Github
Primero lo primero: git y github NO SON LO MISMO. Puede resultar un poco confuso a veces recordar cual es cual pero la gran diferencia es que
1) git es un sistema de control de versiones que esta instalado de manera local (que esta instalado en sus laps pues) mientras que github es una plataforma
2) que permite la colaboracion entre desarrolladores. En pocas palabras github usa git, no al reves. 2) git es mantenido por linux y github por microsoft.

# Local y remoto
En la primera parte hablamos un poco de repositorios locales, pero ¿que significa esto?


# Comandos de conexion
Para poder sincronizar nuestro cambios y mandarlos al repositorio remoto lo hacemos atraves de un par de comandos de git (siempre y cuando todos ellos ya hayan sido commiteados)
- git push: se utiliza para enviar los cambios locales al repositorio remoto. Es decir, actualiza el repositorio remoto con los cambios que has realizado en tu copia local.

¿Qué pasa si se hacen cambios en el remoto?, ¿Se pueden traer a nuestro local? Sí se puede, con los siguientes comandos: 
- git fetch: Este comando se utiliza para obtener los cambios del repositorio remoto sin fusionarlos con tu copia local. Es decir, descarga los cambios del repositorio remoto, pero no los aplica a tu copia local.
- git pull: Este comando se utiliza para obtener los cambios del repositorio remoto y fusionarlos con tu copia local. Es decir, actualiza tu copia local con los cambios que se han realizado en el repositorio remoto.

# Cuidado
Al empezar a trabajar con repositorios locales y remotos junto con nuestro equipo si no existe la comunicación adecuada puede que una o más personas trabajen sobre el mismo archivo;
tal vez alguien borre un archivo y otro este trabajano en el. O peor aun, ¡varias personas estan trabajando sobre la rama principal! Si pasa alguna de estas situaciones lo más probable es que ocurra un conflicto

# Conflictos 
Los conflictos en Git ocurren cuando se fusionan dos ramas que tienen cambios en los mismos archivos. Cuando esto sucede, Git no puede determinar automáticamente qué cambios se deben conservar y cuáles se deben descartar. En este caso, se produce un conflicto de fusión y el usuario debe resolverlo manualmente.
