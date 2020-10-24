# Ejercicio 1. Instalar alguno de los entornos virtuales de node.js (o de cualquier otro lenguaje con el que se esté familiarizado) y, con ellos, instalar la última versión existente, la versión minor más actual de la 4.X y lo mismo para la 0.11 o alguna impar (de desarrollo).

Voy a hacer este ejercicio usando nvm, que voy a instalar siguiendo los pasos indicados en la [documentación del repositorio de nvm](https://github.com/nvm-sh/nvm#install--update-script).

La instalación es bastante sencilla, ya que con una única línea que puedo copiar de la documentación y pegar en mi terminal, descargaré un script y lo ejecutaré, que se encargará de la instalación de nvm y la configuración de variables de entorno. La línea a ejecutar es la siguiente:

> curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.36.0/install.sh | bash

Una vez hecho esto (en Ubuntu) tuve que cerrar y abrir el terminal para que los cambios se tuvieran en cuenta, tal y como se indica en la sección de [*troubleshooting*](https://github.com/nvm-sh/nvm#troubleshooting-on-linux) 

Para utilizarlo, se puede recurrir de nuevo a la [documentación oficial](https://github.com/nvm-sh/nvm#usage), o, como alternativa, escribir *nvm* en la terminal para consultar la ayuda que ofrece:

![Ayuda en la terminal ofrecida por *nvm*](https://github.com/Anglepi/EjerciciosCC/blob/main/Tema2/images/T1E1-nvmTerminal.png)

A continuación, voy a listar todas las versiones de *node.js* para buscar las que cumplan los requisitos expuestos en el enunciado: versión 4.9.1 (la minor más actual de la 4.X), y suponiendo que el enunciado está desactualizado, las últimas versiones de desarrollo a día de hoy son la 15.0.0 y 15.0.1, así que instalaré esta última.

>nvm install 4.9.1
>nvm install 15.0.1

Tras la instalación, consulto las versiones de que dispongo con *nvm ls*

![Versiones de nvm instaladas, consultadas con *nvm ls*](https://github.com/Anglepi/EjerciciosCC/blob/main/Tema2/images/T1E1-nvmls.png)