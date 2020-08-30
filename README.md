# Tarea 00: DCCombateNaval :school_satchel:

## Consideraciones generales :octocat:

Este programa es capaz de simular el juego Combate Naval, jugando contra la computadora. Dentro del programa se puede jugar y ver un registro de los mejores puntajes alcanzados previamente. 

Antes de iniciar el juego, el jugador puede elegir un apodo, y el tamaño del mapa. Ambos sujetos a restricciones.

La computadora puede lanzar bombas normales, mientras que el jugador puede lanzar una bomba normal o una bomba tipo cruz.
Lamentablemente no pude programar el resto de tipos de bombas, ni tampoco que se pueda lanzar la bomba tipo cruz una sola vez por partida.

Cuando alguno de los jugadores hunde todos los barcos enemigos, el juego se termina, se registra el puntaje en un archivo .txt y se vuelve al menú principal.


### Cosas implementadas y no implementadas :white_check_mark: :x:

#### Menús ####
* Menú de Inicio: Hecho completo
* Ranking de puntajes: Hecho completo
* Apodo y tamaño del tablero: Hecho completo
* Menú de juego: Incompleto
    * Rendirse: Completo
    * Lanzar una bomba: Incompleto
        * Selección de coordenada: Incompleto, el programa reconoce cuando una coordenada esta fuera del tablero en la coordenada Y, pero no en la X. Esto debido a que al ingresar una letra que no está en el diccionario, definido en [funciones.py](funciones.py) línea 7, el programa se cierra. Tampoco es capaz de recibir coordenadas inválidas del tipo LetraNumeroLetra.
        * Elegir tipo de bomba: Incompleto
    * Salir del programa: Completo

#### Reglas ####
* Todas se cumplen correctamente, excepto cuando se usa la bomba cruz.

#### Elementos ####
* Tablero: Creado y manipulado correctamente.
* Mapa de Jugador y Oponente: Completo
* Barcos: Completo
* Bombas: Incompleto
    * Bomba normal: Completada
    * Bomba cruz: Esta bomba no fue implementada correctamente. Al acertar a un barco enemigo, no reinicia el turno. Además, se puede lanzar todas las veces que se quiera por partida.
    * Bomba X: No implementada
    * Bomba diamante: No implementada

#### Partida ####
* Crear: Las partidas se crean correctamente.
* Oponente: El oponente funciona correctamente.
* Puntajes: El puntaje es asignado correctamente.


## Ejecución :computer:
El módulo principal de la tarea a ejecutar es  ```main.py```. Además se debe crear los siguientes archivos y directorios adicionales:
1. ```archivo.ext``` en ```ubicación```
2. ```directorio``` en ```ubicación```
3. ...


## Librerías :books:
### Librerías externas utilizadas
La lista de librerías externas que utilicé fue la siguiente:

1. ```sys```: ```exit()```
2. ```copy```: ```deepcopy()```
3. ```random```: ```randint```
4. ```operator```: ```itemgetter```


## Supuestos y consideraciones adicionales :thinking:
Los supuestos que realicé durante la tarea son los siguientes:

1. <Descripción/consideración 1 y justificación del por qué es válido/a> 
2. <Descripción/consideración 2 y justificación del por qué es válido/a>
3. ...

PD: <una última consideración (de ser necesaria) o comentario hecho anteriormente que se quiera **recalcar**>


## Referencias de código externo :book:

Para realizar mi tarea saqué código de:
1. (https://stackoverflow.com/questions/19782075/how-to-stop-terminate-a-python-script-from-running/34029481): este hace que el archivo deje de ejecutarse y está implementado en el archivo [main.py](main.py) en la línea 23 y hace que el programa termine su ejecucuón cuando el usuario elige la opción "[2] Salir" en el menú de inicio


## Descuentos
La guía de descuentos se encuentra [link](https://github.com/IIC2233/syllabus/blob/master/Tareas/Descuentos.md).
