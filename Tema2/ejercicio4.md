# Ejercicio 4. Para la aplicación que se está haciendo, escribir una serie de aserciones y probar que efectivamente no fallan. Añadir tests para una nueva funcionalidad, probar que falla y escribir el código para que no lo haga. A continuación, ejecutarlos desde mocha (u otro módulo de test de alto nivel), usando descripciones del test y del grupo de test de forma correcta. Si hasta ahora no has subido el código que has venido realizando a GitHub, es el momento de hacerlo, porque lo vamos a necesitar un poco más adelante.

He incluido en [oreon](https://github.com/Anglepi/oreon) unos cuantos *assert* para asegurarme de que las variables utilizadas se inicien, y para la funcionalidad nueva que deba fallar el test, he includo una funcion *compruebaGalletas* que se lance cada vez que alguien añada "galletas" a la lista de la compra, y cambie esas galletas por "Galletas Cuetara de las buenas". Tras ejecutar esta funcion, si la variable tiene un valor distinto, falla el test.

Para provocar el fallo del test simplemente hago que la función me devuelva un valor inesperado "Galletas Hacendado de las malas" y haga que salte el assert:

![Codigo que provoca assertion](https://github.com/Anglepi/EjerciciosCC/blob/main/Tema2/images/T2E4-falloAssert.png)

El código para arreglar el fallo del test es sencillo de aplicar, simplemente que la funcion devuelva lo que quiero.

Ahora voy a probar a usar mocha. Incluyo un directorio y fichero test, y lo indico en package.json, donde elaboro mis pruebas. He tenido que incluir un export de la función que devuelve la marca de galletas para poder usarla desde el script de mocha, y tras esto, he lanzado los test y visto que funcionan.

![Test lanzados con mocha funcionando](https://github.com/Anglepi/EjerciciosCC/blob/main/Tema2/images/T2E4-mocha.png)