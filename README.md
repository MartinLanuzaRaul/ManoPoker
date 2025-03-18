# Representación de Cartas Francesas

Este proyecto crea un tipo de objetos que representan Cartas Francesas. Cada carta tiene dos propiedades:

- **palo**: Un carácter que puede ser (c, d, p, t).
- **valor**: Un número del 1 al 13.

Los objetos de este tipo se construyen indicando el palo y el valor. Si hay fallos en los datos, se devuelve un objeto `Carta` con valores `null` en palo y valor.

## Métodos de la Carta

- **darValor(palo, valor)**: Modifica la carta con el palo y valor proporcionados. Si los datos son incorrectos, no se cambia nada en la carta.
- **toString()**: Devuelve una representación textual entendible del valor de la carta. Por ejemplo: "As de Picas".

## Clase Baraja

Además, se implementa otro tipo de objeto: `Baraja`, que representa una baraja de cartas francesas. Tiene las siguientes características:

- La baraja está formada por 52 cartas, almacenadas en un array llamado `cartas`. Al construir la `Baraja`, se rellenan las cartas en el siguiente orden: por palos y cada palo con las cartas del 1 al 13. No se podrá acceder directamente al array fuera del objeto.
  
### Métodos de la Baraja

- **barajar()**: Baraja las cartas, es decir, las desordena de forma aleatoria.
- **toString()**: Permite obtener la baraja en forma de texto para saber qué cartas hay y cómo están ordenadas.
- **reparteCarta()**: Devuelve la última carta de la Baraja, eliminando dicha carta del array de cartas.

## Clase Jugador

El objeto `Jugador` tiene una propiedad `mano` que almacena las cartas que le reparten.

### Métodos del Jugador

- **nuevaCarta(carta)**: Añade cartas al Jugador (hasta un máximo de 5 cartas para jugar al póker).
- **toString()**: Permite obtener las cartas en la mano en forma de texto.
- **jugada()**: Indica la jugada de póker que tiene en la mano (Pareja, Doble pareja, Trío, Escalera, Color, Full, Póker o Escalera de color).

## Página Web

Crea una página web que, utilizando JavaScript, cree una baraja de cartas, las baraje y reparta cinco cartas a un jugador.

La página deberá mostrar la imagen de estas cinco cartas por pantalla (utilizando los ficheros SVG que encontrarás en el fichero `cartas.zip`) e indicar la jugada obtenida por el jugador.
