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
