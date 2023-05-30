# Desafíos de Fundación Formar

## Ejercicios de lógica en Node.JS

Prueba Técnica para ingreso a Formar Sofware Factory

Link del respositorio de GitHub

Estos desafíos tienen como objetivo plasmar tus habilidades lógicas en el ámbito de Node.JS. Contará con 24hs para su desarrollo.

Consideraciones
A continuación están las consignas de los ejercicios.
Cada ejercicio resuelto debe ser agregado a un único respositorio
Cada ejercicio debe estar en un archivo diferente cuyo nombre corresponda con el nombre de la función solicitada en la consigna.

### Primer Ejercicio

Escriba la función **fizz_buzz()** que devuelve un array de 1 a N, pero:

+ Para múltiplos de 3, imprime “Fizz”
+ Para múltiplos de 5, imprime “Buzz”
+ Para múltiplos de 3 y 5 impresiones “FizzBuzz”
  
La función toma un número entero N como parámetro y devuelve la secuencia como un array hasta el índice N.

Ejemplos:

Input: 2
Output: [1,2]

Input: 5
Output: [1,2,"Fizz",4,"Buzz"]

Input: 9
Output: [1,2,"Fizz",4,"Buzz","Fizz",7,8,"Fizz"]

Input: 15
Output: [1,2,"Fizz",4,"Buzz","Fizz",7,8,"Fizz","Buzz",11,"Fizz",13,14,"FizzBuzz"]

### Segundo Ejercicio

Escriba la función **number_cardinality()** que toma un número entero y devuelve una cadena, de la siguiente manera:

1. Devuelve la cadena zero si el número termina en 0
2. Devuelve la cadena five si el número termina en 5
3. Devuelve la cadena even si el número es par (divisible por 2) Y no termina en 0
4. Devuelve la cadena odd si el número es impar (no divisible por 2) Y no termina en 5

Asegúrese de que su cadena de retorno sea exactamente como la anterior, usando letras minúsculas.

Ejemplos:

Input: 100
Output: zero

Input: 88
Output: even

Input: 155
Output: five

Input: 99
Output: odd

### Tercer Ejercicio

Crear la función **range_vision()** que, dado un entero no negativo, determine si hay al menos un dígito 1 en el entero que tiene el valor de visualización más bajo de todos los dígitos del entero. La función debe devolver un booleano: **true** cuando un dígito 1 tiene el valor de vista más bajo en el número dado, **false** de lo contrario.

Imagine un número entero no negativo, digamos 34315. Cada dígito en el número entero tiene un llamado **rango de visión** . El primer dígito, 3, tiene un rango de visión de 3. En otras palabras, puede 3 "ver" 3 dígitos a cada lado de sí mismo. En nuestro ejemplo, puede mirar a la derecha de sí mismo y ver 4, 3 y 1. A la izquierda, no hay nada. **El rango de visión de cada dígito es su propio valor.**

Ahora bien, el **rango de visión** de un dígito define el llamado **valor de visión**, que es la suma de los dígitos dentro del **rango de visión.** Entonces, el valor de visión del primer dígito, 3 es 4+3+1=**8.** Para el segundo dígito, 4 el valor de visión es 3+3+1+5=**12.**

Ejemplos:

Para el número **34315**:

Dígito: 3
Puede ver a la izquierda: -
Puede ver a la derecha: 431
Valor de la visión:4 + 3 + 1 = 8

Dígito: 4
Se puede ver a la izquierda: 3
Se puede ver a la derecha: 315
Valor de la visión:3 + 3 + 1 + 5 = 12

Dígito: 3
Puede ver a la izquierda: 34
Puede ver a la derecha: 15
Valor de la visión:3 + 4 + 1 + 5 = 13

Dígito: 1
Se puede ver a la izquierda: 3
Se puede ver a la derecha: 5
Valor de la visión:3 + 5 = 8

Dígito: 5
Puede ver a la izquierda: 3431
Puede ver a la derecha: -
valor de la visión:3 + 4 + 3 + 1 = 11

¿Hay un dígito 1 en el número entero para el cual el **valor de visión** es mínimo?

Sí, 8 es el valor mínimo de visión, tanto para el primer 3 como para el 1. Eso satisface los criterios, por lo que la función devuelve true.
