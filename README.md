# Matemáticas Discretas 

## Lógica 
**¿Que es?**
La lógica es uno de los temas mas importantes no solo en las matemáticas si no en todo lo que nos rodea.
La lógica es todo lo que tiene sentido es decir el estudio del razonamiento

### Lógica proposicional simbólica o matemática
Es la lógica que proporciona o afirma 
Las proposiciones son sentencias o oraciónes, un enunciado al que yo le puedo dar valor de verdadero o falso 

**Ejemplo**
El dia esta soleado

### Proposiciones Simples 
Son proposiciones que constan de una sola oración y se representan con letras minúsculas

    p = Juan es arquitecto
    q = Mi zapato es rojo

### Proposiciones Compuestas 
Estas están formadas de dos o mas proposiciones simples 

**Ejemplo**

Sergio es deportista y Javier es ingeniero 

Aquí podemos ver que están unidas por la letra y

|Sergio es deportista|y|Javier es ingeniero|
|:-:|:-:|:-:| 

## Conectores lógicos 

|Conector lógico|Símbolo|Nombre|
|:-:|:-:|:-:|
|y|∧|Conjunción|
|o|∨|Disyunción débil|
|o...o|Δ|Disyunción fuerte|
|Si... entonces ..|→|Implicación|
|Si y solo si|↔|Equivalencia|
|No es verdad|~|Negación|

### Conjunción
|p|y|q|
|:-:|:-:|:-:|
|Esta lloviendo|y|Hace frio|

|p|q|p∧q|
|:-:|:-:|:-:|
|V|V|V|
|V|F|F|
|F|V|F|
|F|F|F|

Lo que esto nos dice es que la proposición solo es verdadera si las dos proposiciónes son verdaderas 

### Disyunción débil

|p|o|q|
|:-:|:-:|:-:|
|Esta lloviendo|o|Hace frio|

|p|q|p∨q|
|:-:|:-:|:-:|
|V|V|V|
|V|F|V|
|F|V|V|
|F|F|F|

esto nos quiere decir que va a ser falso solo si las 2 son falsas

### Disyunción fuerte

|o|p|o|q|
|:-:|:-:|:-:|:-:|
|o|Esta lloviendo|o|Hace frio|

|p|q|pΔq|
|:-:|:-:|:-:|
|V|V|F|
|V|F|V|
|F|V|V|
|F|F|F|

Esta nos quiere decir que una de las dos deben cumplirse pero no las dos y tampoco pueden ser las dos falsas

### Implicación 

|Si|p|entonces|q|
|:-:|:-:|:-:|:-:|
|Si|Esta lloviendo|entonces|hace frio|

|p|q|p→q|
|:-:|:-:|:-:|
|V|V|V|
|V|F|F|
|F|V|V|
|F|F|V|

La única forma en que sea falsa es que este lloviendo y no haga frio es decir que la primera sea verdadera y la segunda sea falsa 

### Equivalencia

|p|entonces|q|
|:-:|:-:|:-:|
|Esta lloviendo|Si y solo si|hace frio|

|p|q|p↔q|
|:-:|:-:|:-:|
|V|V|V|
|V|F|F|
|F|V|F|
|F|F|V|

Solo va a ser verdadero si ambas son verdaderas o ambas son falsas 

### Negación 

|~p|
|:-:
|No Esta lloviendo|

|p|~p|
|:-:|:-:|
|V|F|
|F|V|

Lo que hace la negación es negar lo que esta pasando 

## Tablas de verdad 

### Tautología
La tautología se da cuando todas nuestras respuestas son verdaderas

|p|q|Formula|
|:-:|:-:|:-:|
|V|V|**V**|
|V|F|**V**|
|F|V|**V**|
|F|F|**V**|

### Contradicción
La contradicción se da cuando todas nuestras respuestas son falsos
|p|q|Formula|
|:-:|:-:|:-:|
|V|V|**F**|
|V|F|**F**|
|F|V|**F**|
|F|F|**F**|

### Contingencia
La contingencia es cuando nuestras respuestas son entre verdaderas y falsas 

|p|q|Formula|
|:-:|:-:|:-:|
|V|V|**V**|
|V|F|**F**|
|F|V|**V**|
|F|F|**F**|

#### Construcción tabla de verdad
**p→(p∧~p)**

|p|~p|p∧~p|p→(p∧~p)|
|:-:|:-:|:-:|:-:|
|V|F|F|F|
|F|V|F|V|

**(p∨q)∨~q**

|p|q|p∧~q|~q|(p∨q)∨~q|
|:-:|:-:|:-:|:-:|:-:|
|V|V|V|F|V|
|V|F|V|V|V|
|F|V|V|F|V|
|F|F|F|V|V|

**Ejercicio**

Si se conoce que (q∨~r)∨p es falso. Determinemos
(~r∨~p)→(p→~p)

Para poder resolver esto primero tenemos que encontrar el valor de (q∨~r)∨p, ya que el ejercicio nos dice que es falso y ya que es una disyunción quiere decir que ambas son falsas

|(q∨~r)|∨|p|=|F|
|:-:|:-:|:-:|:-:|:-:
|F|o|F|

con esto encontramos el valor de p que es F

y seguimos de igual manera con lo siguiente hasta encontrar el valor de q y de r

|q|∨|~r|=|F|
|:-:|:-:|:-:|:-:|:-:
|F|o|F|

entonces tenemos que 

    p = F
    q = F
    r = V

y a continuación remplazamos estos valores en lo que nos pide resolver 

|(~r ∨ ~p)|→|(p → ~p)|
|:-:|:-:|:-:|
|~V ∨ ~F|→|(F → ~ F)
|F ∨ V|→|F → V|
|V|→|V|
||V||

**Ejercicios**

1. ((p∧(q→r)))∨((q∧~r)↔~r)

|p|q|r|q→r|p∧(q→r)|~r|q∧~r|(q∧~r)↔~r|((p∧(q→r)))∨((q∧~r)↔~r)
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|V|V|V|V|V|F|F|V|V|
|V|V|F|F|F|V|V|V|V|
|V|F|V|V|V|F|F|F|V|
|V|F|F|F|F|V|F|V|F|
|F|V|V|V|F|F|F|V|V|
|F|V|F|V|F|V|V|V|V|
|F|F|V|V|F|F|F|V|V|
|F|F|F|V|F|V|F|F|F|

## Introducción a los conjuntos 
 un conjunto es una colección de elementos con características similares considerada en sí misma como un objeto. Los elementos de un conjunto, pueden ser las siguientes: personas, números, colores, letras, figuras, etc. Se dice que un elemento (o miembro) pertenece al conjunto si está definido como incluido de algún modo dentro de él.

### Relación de pertenencia
Quiere decir que algo pertenece o no a un conjunto y se expresa de la siguiente manera 

|Pertenece|No Pertenece|
|:-:|:-:|
|∈|∉|

**Ejemplos**
A = {1,2,3,4,5}

1 **∈** A,
3 **∈** A,
7 **∉** A

### Determinación de un conjunto
Es la forma a la que llamamos al conjunto y existen dos formas:
* **Por extension**: Es cuando conocemos a los elementos del conjunto individualmente 
* **Por comprensión**: Es cuando conocemos las cualidades del conjunto 

|Por extension|Por comprensión|
|:-:|:-:|
|A={2,4,6}|A={x x es una vocal}|

También los conocemos por conjuntos finitos y infinitos 
|Finitos|Infinitos|
|:-:|:-:|
|Por extension|Por compresión|

### Cardinalidad 

Es el número de elementos que forma el conjunto 

### Subconjuntos 
Es un conjunto dentro de otro conjunto 

**Ejemplo**

Supongamos que A y B son conjuntos. Si dado elemento de B esta contenido en A e dice que B es un subconjunto de A y se representa con ⊆

A = {Abecedario} B = {Vocales}

B ⊆ A

### Operaciones entre conjuntos 
|Símbolo|Nombre|Concepto|
|:-:|:-:|:-:|
|⋃|Unión|Los elementos de un conjunto **A** se unen a los de un conjunto **B**|
|⋂|Intersección|Son los elementos que se repiten tanto en **A** como en **B**|
|–|Diferencia|Es la resta de los elementos entre dos conjuntos es decir los elementos que no se repiten| 
|Cª|Complemento|Son los elementos que le hacen falta al conjunto para ser el conjunto universal|
