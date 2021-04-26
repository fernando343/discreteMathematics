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


