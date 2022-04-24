# MarkDown
## Resumen de sintaxis

|1. Elementos de bloque|2. Elementos de linea|3. Elementos varios|
|---|---|---|
|- [Párrafos y saltos de línea](#Parrafos-y-saltos-de-lineas)|- [Énfasis](#Enfasis)|- [Links automáticos](#Links-automaticos)|
|- [Encabezados](#Encabezados)|- [Links o enlaces](#Links-o-enlaces)|- [Omitir Markdown](#Omitir-Markdown)|
|- [Citas](#Citas)|- [Código](#Codigo)||
|- [Listas](#Listas)|- [Imágenes](#Imagenes)||
|- [Codigo de bloque](#Codigo-de-bloque)|||
|- [Reglas horizontales](#Reglas-horizontales)|||  

# Elementos de bloque
## Parrafos y saltos de lineas
Al igual que sucede con HTML, Markdown no soporta dobles líneas en blanco, así que si intentas generarlas estas se convertirán en una sola al procesarse.

Para realizar un salto de línea y empezar una frase en una línea siguiente dentro del mismo párrafo, tendrás que pulsar dos veces la barra espaciadora antes de pulsar una vez intro.

## Encabezados
Se establecen mediante el uso de la `#`
```
# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6
```

Ejemplos:

# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6

## Citas
Las citas se generar utilizando el carácter mayor que `>` al comienzo del bloque de texto.
Si la cita en cuestión se compone de **varios párrafos**, deberás añadir el mismo símbolo `>` al comienzo de cada uno de ellos.

```
> Esto es una cita. Y no se quien puede ser el autor...
>
> Continuacion de la cita en otro parrafo. -Anonymous
```

> Esto es una cita. Y no se quien puede ser el autor...
>
> Continuacion de la cita en otro parrafo. - Anonymous

## Listas
### Desordenadas
Para crear listas desordenadas utiliza `*` asteriscos, `-` guiones, o `+` símbolo de suma.

Para generar listas anidadas dentro de otras, simplemente tendrás que añadir **cuatro espacios** en blanco antes del siguiente `*`, `-` o `+`.

Ejemplos:
```
* Lista desordenada 1
    + Sublista desordenada 1
    - Sublista desordenada 2
- Lista desordenada 2
+ Lista desordenada 3
```
* Lista desordenada 1
    + Sublista desordenada 1
    - Sublista desordenada 2
- Lista desordenada 2
+ Lista desordenada 3

### Ordenadas
Para crear listas ordenadas debes utilizar la sintaxis de tipo: «número.» **(1.)** Al igual que ocurre con las listas desordenadas, también podrás anidarlas o combinarlas.

Ejemplos:
```
1. Elemento de lista 1
2. Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        1. Elemento de lista 5
        2. Elemento de lista 6
```
1. Elemento de lista 1
2. Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        1. Elemento de lista 5
        2. Elemento de lista 6

## Codigo de bloque
Si quieres crear un bloque entero que contenga código. Lo único que tienes que hacer es encerrar dicho párrafo entre dos líneas formadas por tres ~ virgulillas.

Ejemplo:
```
~~~
Creando códigos de bloque.
Puedes añadir tantas líneas y párrafos como quieras. 
~~~
```
~~~
Creando códigos de bloque.
Puedes añadir tantas líneas y párrafos como quieras. 
~~~

## Reglas horizontales
Para crearlas, en una línea en blanco deberás incluir tres de los siguientes elementos: asteriscos (***), guiones (---), o guiones bajos (___).

Ejemplos:

```
***
---
___
```
***
---
___

# Elementos de linea
## Enfasis
Markdown utiliza asteriscos (*) o guiones (_) bajos para enfatizar.
Simplemente tendrás que envolver palabras o textos en éstos símbolos para conseguir *cursivas* o **negritas**.

|Markdown|Resultados|
|---|---|
|\*cursiva\*|*cursiva*|
|\_cursiva\_|_cursiva_|
|\*\*negrita\*\*|**negrita**|
|\_\_negrita\_\_|__negrita__|
|\*\*\*negrita y cursiva\*\*\*|***negrita y cursiva***|
|\_\_\_negrita y cursiva\_\_\_|___negrita y cursiva___|

## Links o enlaces
### En linea
Son los enlaces de toda la vida. Como su nombre indica, se encuentran en línea con el texto.

Se crean escribiendo la palabra o texto enlazada entre [] corchetes, y el link en cuestión entre () paréntesis.

|MarkDown|Resultado|
|---|---|
|\[enlace en línea\]\(http://www.limni.net)|[enlace en línea](http://www.limni.net)|

### Internos
Son los enlaces dentro de un mismo documento, como por ejemplo los enlaces del indice de este documento a las distintas partes del mismo.

Se crean escribiendo la palabra o texto enlazada entre [] corchetes, y el nombre del encabezado entre () paréntesis, con un `#` delante.

|MarkDown|Resultado|
|---|---|
|\[enlace interno\]\(\#Nombre-encabezado-interno)|[enlace interno](#Internos)|

### Como referencia
En tu texto enlazarás palabras o códigos concretos (formados por letras y/o números), que en otro lugar más apartado de tu documento tendrás definidos como determinadas URL.

Ejemplo:
~~~
Me llamo Javier Cristóbal y tengo un blog sobre [productividad mac][blog].
En dicha [web][blog] recopilo artículos sobre todo lo relacionado con automatización, gestión y eficiencia.
[blog]: http://limni.net/blog/
~~~
Me llamo Javier Cristóbal y tengo un blog sobre [productividad mac][blog].
En dicha [web][blog] recopilo artículos sobre todo lo relacionado con automatización, gestión y eficiencia.
[blog]: http://limni.net/blog/

La referencia `[blog]` puede estar incluida en cualquier parte del documento, así puedes organizarte mejor y de una manera más limpia, recopilando todas tus referencias en un mismo lugar.

## Codigo
### Codigo puro
La forma más sencilla de escribir código en Markdown es envolver el texto entre dos comillas sencillas \` . Esto se corresponde con la etiqueta HTML `<code>`.

Ejemplo:

\` Esto es una linea de codigo \`

` Esto es una linea de codigo `

### Codigo preformateado `<pre>`
La otra manera de añadir código en Markdown es comenzar el párrafo con cuatro espacios en blanco. Esto se corresponde con la etiqueta HTML `<pre>`

Ejemplo:

    Esto es una linea de codigo
    
## Imagenes
Insertar una imagen con Markdown se realiza de una manera prácticamente idéntica a insertar links.
Solo que en este caso, deberás añadir un símbolo de `!` exclamación al principio y el enlace no será otro que la ubicación de la imagen.

El `texto alternativo` es lo que se mostraría si la carga de la imagen fallase.
También podrás añadir un `título alternativo` entrecomillándolo al final de la ruta. Esto sería el título mostrado al dejar el cursor del ratón sobre la imagen.

Ejemplo:

    ![Texto alternativo](/ruta/a/la/imagen.jpg "Título alternativo")
    
![Logo de MarkDown](https://icon-library.com/images/markdown-icon/markdown-icon-24.jpg "MarkDown LOGO")
    
# Elementos varios
# Links automaticos
Para generar links automáticos tan solo tendrás que rodearlos con los símbolos < >.

Ejemplo:

`<http://www.google.es>`

<http://www.google.es>

## Omitir MarkDown
Si has llegado hasta aquí es probable que te estés preguntando cómo he conseguido escribir ciertos símbolos como \* asteriscos o \_ guiones bajos, sin que Markdown los interprete para convertirlos en negritas, cursivas…
Se trata de la barra invertida \.

Sencillo, escribiéndola justo delante de cualquiera de los elementos que verás a continuación una barra invertida `\`, los mismos no tendrán efecto a la hora de convertirse en negritas, cursivas, links…

```
\  barra invertida
`  acento invertido
*  asterisco
_  guión bajo
{} llaves
[] corchetes
() paréntesis
#  almohadilla
+  símbolo de suma
-  guión
.  punto
!  exclamación
```
