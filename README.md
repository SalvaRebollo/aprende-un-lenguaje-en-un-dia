# Aprende un lenguaje de programación en un día (ejercicio voluntario para subir nota).

## Introducción

Cuando te sacaste el carnet de conducir, aprendiste las normas de circulación así como los fundamentos básicos para manejar un coche: volante, marchas, freno, acelerador, embrague, retrovisores... Seguramente, el coche que conduces ahora es diferente al que utilizaste para aprender a conducir, no obstante, lo puedes llevar sin problema. Cada coche tiene sus peculiaridades, pero quien sabe manejar un automóvil, puede adaptarse a las medidas, tacto y comportamiento de un vehículo en cuestión de horas.

Aprender a programar es como aprender a conducir. Si tienes una base sólida de programación y sabes manejar con soltura los tipos de datos, bucles, arrays, clases, métodos, etc. podrás pasar de un lenguaje a otro en un período relativamente corto, simplemente tendrás que adaptarte a la sintaxis y a las peculiaridades del nuevo lenguaje.

Con este ejercicio se pretende despertar el interés por otros lenguajes de programación distintos al que el alumno está estudiando como primer lenguaje.

Sigue los pasos que se indican a continuación.

## Creación del equipo

Este ejercicio se debe hacer en grupos de 3 alumnos. Uno de ellos será el representante del grupo.

## Forkea forkea

El representante del grupo debe hacer un *fork* de este repositorio para utilizarlo como base.

## Añadiendo colaboradores

El encargado del grupo deberá añadir como colaboradores del repositorio *forkeado* a los otros dos miembros, para trabajar todos sobre los mismos archivos. Cuando alguien es colaborador en un repositorio, puede hacer *push* a él sin necesidad de pedir permiso o hacer *pull request*.

Para añadir colaboradores hay que hacer click en la pestaña *Settings* y seleccionar luego *Collaborators* en el menú.

## Miembros del grupo

Escribe aquí los miembros del grupo. El primero es el representante o encargado.

Nombre de equipo: The Brainfuckers.

* Salvador Rebollo Benítez  <--Cabecilla
* Nacho Espejo García
* Jose Antonio Ruíz Mostazo

## Lenguaje de programación

El profesor llevará una cajita llena de papelitos con los nombres de distintos lenguajes de programación. Los encargados de cada grupo meterán la mano en la caja y sacarán dos papelitos, de los cuales el grupo elegirá uno. Se permite hacer intercambio de papelitos entre grupos.

Escribe el lenguaje de programación elegido por el grupo.

* Smalltalk

Los papelitos se han recortado de este [documento](lenguajes_de_programacion.pdf).

## Información sobre el lenguaje

<img width="1080px" src="/imagenes/customLogo.png">

* **¿Cuándo se creó?** 
Su desarrollo comenzó en 1969 y se hizo público en 1980.

* **¿Para qué se creó?**
Los orígenes de SmallTalk se encuentran en las invetigaciones para a creaciónn de un sistema informático orientado a la eduacación. El objetivo era crear un sistema que permitiese expandir la creatividad de sus usuarios, proporcionando un entorno para la experimentación, creación e investigación.

* **¿Qué es?**
SmallTalk es un lenguaje de programación orientado a objetos puro, con recolector de basura, también fue uno de los primeros lenguajes de programción gráficos, creado por Alan Kay de Xerox PARC y otros. Mantiene la idea de que "todo es un objeto, es decir, cuando ingresamos a un entorno de SmallTalk, lo que hacemos es enviarles "mensajes" para esperar una respuesta.
Al considerar todos los elementos como objetos, podemos decir que éstos tiene 4 características comunes:
Memoria Propia, Comunicación con otros objetos, Posibilidad de "heredar" las características de otros objetos, Posibilidad de procesamiento.


## Herramientas de desarrollo

Primero comprobamos que tenemos gst instalado, en la consola tecleamos:
```console
$ whereis gst 
gst:
```
Si no es así procedemos a la instalación con la siguiente línea:
```console
$ sudo apt-get install gnu-smalltalk
```

## Poniendo en práctica el lenguaje

Pon en práctica el lenguaje de programación realizando los siguientes ejercicios. Para cada uno de los ejercicios, pega el código fuente de la solución y una captura de pantalla.

### 1. ¡Hola mundo! :heavy_check_mark:

Realiza un programa que muestre por pantalla la frase **¡Hola mundo!**.

```Smalltalk
"Programa Hola Mundo"
 
'Hola Mundo!' printNl !
```

<img width="720px" src="/imagenes/holamundo.png">

### 2. Pirámide :heavy_check_mark:

Dada una altura introducida por el usuario, realiza un programa que pinte una pirámide a base de asteriscos con la altura indicada.

```Smalltalk
|altura alturaIntroducida espacios i j| 
altura:=1.
Transcript show:'Introduce una altura:'.
alturaIntroducida:=stdin nextLine asInteger.
espacios:=alturaIntroducida-1.
i:=0.
j:=1.

[altura <= alturaIntroducida] whileTrue:[ 
	i:=1.
	[i<=espacios] whileTrue:[ 
 	
	Transcript show:' '.
	
 	i:=i+1.
	].

	j:=1.
	[j<(altura*2)] whileTrue:[ 
 	
	Transcript show:'*'.

 	j:=j+1.
	].
Transcript cr.
altura:=altura+1.
espacios:=espacios-1.
].
Transcript cr.
```

<img width="720px" src="/imagenes/piramide.png">

### 3. Arrays y números aleatorios :construction: Under development :construction:

Realiza un programa que rellene un array (o una estructura similar) con 20 números enteros aleatorios entre 1 y 100 y que seguidamente los muestre por pantalla. A continuación, se deben pasar los números primos a las primeras posiciones del array y los no primos a las posiciones restantes. Muestra finalmente el array resultado.

## Presentación de resultados

Cada equipo explicará al resto de la clase lo aprendido durante la realización del ejercicio. Todos los miembros de cada equipo deben participar en la explicación. Se puede utilizar como material de base para la presentación el repositorio de GitHub.

## Recompensa

* Todos los alumnos que realicen correctamente la actividad tendrán 0'25 puntos extra en la nota del trimestre.

* Los miembros del equipo más votado ganarán un premio.

:star: Si te ha gustado este ejercicio, dale una estrellita al [repositorio original](https://github.com/LuisJoseSanchez/aprende-un-lenguaje-en-un-dia).

