# Tarea 00: DCCombateNaval

## Consideraciones generales

* Este programa es capaz de simular el juego Combate Naval, jugando contra la computadora. Dentro del programa se puede jugar y ver un registro de los mejores puntajes alcanzados previamente. 

* Antes de iniciar el juego, el jugador puede elegir un apodo, y el tamaño del mapa. Ambos sujetos a restricciones.

* La computadora puede lanzar bombas normales, mientras que el jugador puede lanzar una bomba normal o una bomba tipo cruz.
Lamentablemente no pude programar el resto de tipos de bombas, ni tampoco que se pueda lanzar la bomba tipo cruz una sola vez por partida.

* Cuando alguno de los jugadores hunde todos los barcos enemigos, el juego se termina, se registra el puntaje en un archivo .txt y se vuelve al menú principal.


### Cosas implementadas y no implementadas

* #### Menús ####
    * **Menú de Inicio**: Hecho completo.
    * **Ranking de puntajes**: Hecho completo.
    * **Apodo y tamaño del tablero**: Hecho completo.
    * **Menú de juego**: Incompleto.
        * **Rendirse**: Completo.
        * **Lanzar una bomba**: Incompleto.
            * **Selección de coordenada**: Incompleto, el programa reconoce cuando una coordenada esta fuera del tablero en la coordenada Y, pero no en la X. Esto debido a que al ingresar una letra que no está en el diccionario, definido en [funciones.py](funciones.py) línea 7, el programa se cierra. Tampoco es capaz de recibir coordenadas inválidas del tipo LetraNumeroLetra.
            * **Elegir tipo de bomba**: Incompleto.
        * **Salir del programa**: Completo.

* #### Reglas ####
    * Todas se cumplen correctamente, excepto cuando se usa la bomba cruz.

* #### Elementos ####
    * **Tablero**: Creado y manipulado correctamente.
    * **Mapa de Jugador y Oponente**: Completo.
    * **Barcos**: Completo.
    * **Bombas**: Incompleto.
        * **Bomba normal**: Completada.
        * **Bomba cruz**: Esta bomba no fue implementada correctamente. Al acertar a un barco enemigo, no reinicia el turno. Además, se puede lanzar todas las veces que se quiera por partida.
        * **Bomba X**: No implementada.
        * **Bomba diamante**: No implementada.

* #### Partida ####
    * **Crear**: Las partidas se crean correctamente.
    * **Oponente**: El oponente funciona correctamente.
    * **Puntajes**: El puntaje es asignado correctamente.


## Ejecución
El módulo principal de la tarea a ejecutar es  ```main.py```.


## Librerías
### Librerías externas utilizadas
La lista de librerías externas que utilicé fue la siguiente:

1. ```sys```: ```exit()```
2. ```copy```: ```deepcopy()```
3. ```random```: ```randint```
4. ```operator```: ```itemgetter```


## Referencias de código externo

Para realizar mi tarea saqué código de:
1. (https://stackoverflow.com/questions/19782075/how-to-stop-terminate-a-python-script-from-running/34029481): Este hace que el archivo deje de ejecutarse y está implementado en el archivo [main.py](main.py) en la línea 23 y hace que el programa termine su ejecucuón cuando el usuario elige la opción "[2] Salir" en el menú de inicio.
2. (https://www.geeksforgeeks.org/copy-python-deep-copy-shallow-copy/): Este código permite copiar una lista, sin compartir un espacio en la memoria. Está implementado en el archivo [funciones.py](funciones.py) en la línea 22.
3. (# https://stackoverflow.com/questions/38891066/how-to-create-10-random-x-y-coordinates-in-a-grid-using-python/38891529): Este código, crea coordenadas aleatorias (x, y) para elegir la posición de los barcos. Está implementado en el archivo [funciones.py](funciones.py) en la línea 26.
4. (https://stackoverflow.com/questions/8023306/get-key-by-value-in-dictionary): El codigo utilizado permite obtener la llave en un diccionario a partir del valor de esta. Está implementado en el archivo [funciones.py](funciones.py) en la línea 132.
5. (https://stackoverflow.com/questions/4174941/how-to-sort-a-list-of-lists-by-a-specific-index-of-the-inner-list): El codigo permite ordenar una lista de listas, usando como parámetro un item de las listas. Esta implementado en el archivo [funciones.py](funciones.py) en la línea 151.


## Descuentos
La guía de descuentos se encuentra [link](https://github.com/IIC2233/syllabus/blob/master/Tareas/Descuentos.md).
