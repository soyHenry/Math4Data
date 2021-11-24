<img  src='../logo.png' height='70px'>

# Introducción a Cálculo I

## Filosofia de este curso

Si la matemática nunca fue lo tuyo, te invitamos a olvidar lo aprendido y a “empezar de cero”! El objetivo de este curso es de revisar conceptos fundamentales que van a ayudarte a entender mejor temas claves a la data/ data science como lo son la probabilidad, estadística o machine learning. 
Como hoy en día los cálculos los hace la computadora, y estamos conscientes de ello, no vamos a insistir en la resolución de ejercicios complejos que no solo lleva tiempo sino que puede traer frustración innecesaria. 
Por ello, abordaremos los temas seleccionados desde lo conceptual, con ejemplos precisos e invitandote a abrir la mente hacia una nueva manera de aprender matemática.
Por último, el fin de este documento es presentar un temario variado de conceptos que nos parecen importantes a tener en cuenta. Para que sea de fácil lectura, los temas no están desarrollados en gran profundidad. Animate a googlear los temas que te interesen o que necesiten más explicación!

Vamos!


## Temario

* Conceptos generales
* Funciones
* Gráficos
* Ecuación de la recta
* Continuidad
* Derivabilidad
* Operar con log, raiz, potencias
* Función discreta: concepto

## Conceptos generales

### Tipos de números

Según su naturaleza; existen los siguientes tipos de números

* **Naturales**: 0, 1, 2, … (enteros, es decir sin coma, mayores o iguales que cero)
* **Enteros**: -2, -1, 0, 1…(Naturales + los enteros negativos)
* **Reales**
  * *Racionales*: números con coma que pueden representarse como una fracción 
  1.223, 100002.44
  * *Irracionales*: números con coma que NO pueden representarse como una fracción y tienen infinitos digitos tras la coma 
  Típicos ejemplos son el famoso “Pi”, “e” o el “numero de oro” (mas info http://xtec.cat/~fgonzal2/curio_irrac.html)

Cada uno de estos grupos, o conjuntos, tienen infinitos elementos. Es decir, para cualquier numero elegido siempre va a haber un numero mayor (o menor en el caso de un negativo). El concepto de infinito es recurrente en matematica.

Una fracción es una división entre dos números. En muchas aplicaciones se usa la nomenclatura XYdonde X e Y son diferentes números Enteros. Por ejemplo, en vez de 0.5 se puede escribir 12y se lee “un medio” o mundanamente “la mitad”. Mas en http://hnaranjo.com/blog/numeros-racionales/.

Como podes imaginar, la ventaja de los números racionales es que por mas “largos” que sean (largos=digitos después de la coma) siempre se pueden representar en su totalidad. En cambio, un número irracional no se puede representar totalmente en una cantidad finita de digitos.

Cada tipo tiene usos diferentes. Por ejemplo, en programación un número entero no se guarda en memoria de la misma manera que un racional. Otra diferencia existe en el uso de distintos tipos de números para representar la realidad a través de datos en algoritmos de machine learning. 

Si buscas en internet vas a encontrar más categorías como los complejos, imaginarios, periódicos cuya definición es interesante pero menos relevante a este curso. 

En el siguiente grafico vas a encontrar las relaciones entre los conjuntos mencionados.

<img  src='./figuras/type_num.png' height='370px'>

### Porcentajes

Rápidamente, revisaremos cómo calcular porcentajes (o proporciones, o fracciones).

Usamos porcentajes para relacionar cualquier número a 100. Cuando decimos “el 30% de 2000” nos referimos a la cantidad que sea a 2000 como lo es 30 a 100. Hay varias formas de calcularlo:

* regla de 3:  

        100 ----- 30
        2000 ------ X
        
        X=30*2000 / 100 = 600

* fracciones:

        30% es lo mismo que 30/100, entonces para calcular el 30% de 2000 hacemos 30/100* 2000 (regla para recordar, “de” en matemática se traduce a “*”) que es igual a 30/100 * 200 = 600

* número decimal:

       30% es lo mismo que 30/100que es lo mismo que 0,3.
       Entonces, podemos hacer directamente 0,3 * 2000 = 600


Naturalmente, las 3 opciones llevan al mismo cálculo y resultado. Podes elegir la que te resulte más sencilla.			

Por último, un porcentaje no es necesariamente un número menor. Por ejemplo, el 230% de 2000 es

    X=230*2000 / 100 = 4600
    230/100* 2000 = 4600
     2,3 * 2000 = 600

o también “el doble (200%) más el 30%” o sea 2000*2+600.

### Geometría: Ángulos y trigonometría 

Un ángulo se puede definir como la medida de abertura entre dos rectas. El concepto se usa mucho en análisis matemático y álgebra ya que mide la relación entre distintos elementos en el espacio, o la inclinación de una recta respecto a la horizontal. 

En grados, una abertura nula corresponde a 0°. Cuando dos rectas tienen un ángulo de 0, se dice que son paralelas. Luego podemos ir agrandando el ángulo hasta 90°, donde los dos vectores son perpendiculares (ver en la imagen). Un cuadrado tiene cuatro ángulos de 90° que se llaman también ángulos rectos. Si seguimos agrandando en un momento volvemos a crear una horizontal, que es equivalente a dos veces una abertura recta o sea 180°. Con esta lógica, el ángulo se puede seguir agrandando hasta la posición inicial habiendo recorrido 360°. 360° corresponde entonces a la misma posición que 0°, pero indicando que se ha recorrido el círculo entero una vez (lo cual tiene aplicaciones en casos donde se analizan por ejemplo movimientos en función del tiempo).

<img  src='./figuras/angles.png' height='370px'>

Solo porque nociones como seno y coseno son bastante usadas en cálculo y álgebra, vamos a refrescar los conceptos yendo a los puntos claves. 

Tomando cualquier ángulo entre dos rectas del ejemplo anterior, podemos trazar una recta (azul) más entre ambas y formar un triángulo. 

<img  src='./figuras/angle.png' height='170px'>

Si además la recta que trazamos forma un ángulo recto con alguna de las existentes (señalado en el ejemplo con un cuadradito), tenemos lo que se llama un triángulo recto el cual es muy utilizado entre otras cosas, por su seno y coseno.

Esquema de un ángulo recto y el nombre que se les da a sus lados:

<img  src='./figuras/triangle.png' height='70px'>


Cada uno de los lados (X,Y,H) tienen una medida (por ejemplo, en centímetros). En matemática, cuando nos referimos a la medida de un segmento usamos || alrededor de su nombre. En este caso, |X| es la medida del lado que hemos llamado X, por ejemplo 1,5 cm. Con estos 
conceptos en mente, seno, coseno y tangente del <span style="color:pink"> ángulo </span> en cuestión son:

**coseno**=|X|/|H| (la medida del lado contiguo, aca llamado X, dividido la medida del lado H)

**seno**=|Y|/|H| (la medida del lado opuesto, aca llamado Y, dividido la medida del lado H)

**tangente**=|Y|/|X| (que es lo mismo que seno/coseno)

Yendo un poco más allá: imaginemos un triángulo como este, donde |H|=1. En este caso, tenemos directamente que
coseno=|X|, seno=|Y| y tangente=|Y|/|X|

Si H mide 1, X e Y miden imperativamente menos que 1 (tiene lógica!), por lo que el seno y el coseno pueden valer entre 0 y 1 (también valores negativos, entre 0 y -1 para ángulos entre 180° y 360°). 
Si imaginamos <font color="pink"> ángulo </font> tan chico como sea posible (0°), entonces el lado Y desaparece (|Y|=0) y |X|=|H|=1. 
Es decir, el seno(0°)=0 y el coseno(0°)=1. Con la misma lógica, si abrimos <span style="color:pink"> ángulo </span> hasta los 90° sucede lo contrario donde X desaparece (|X|=0) y |Y|=|H|=1. 
Entonces, el seno(90°)=1 y el coseno(90°)=0. En la sección Gráficos, veremos qué forma tienen esas relaciones visualmente.

## Funciones

Uno de los conceptos más importante del análisis matemático, y sin dudas el más importante de este módulo, es el de **función**. 

## Gráficos
## Ecuación de la recta
## Continuidad
## Derivabilidad
## Operar con log, raiz, potencias
## Función discreta: concepto