# Introducción a JavaScript: Conceptos Básicos

En esta primera clase, exploraremos los conceptos básicos de JavaScript, un lenguaje de programación ampliamente utilizado en el desarrollo web. Aprenderemos sobre variables, operadores, estructuras de control y más. ¡Comencemos!

## Contenido

1. *Variables*: Las variables son contenedores que nos permiten almacenar y manipular datos en JavaScript. Podemos declarar una variable utilizando la palabra clave `var`, `let` o `const`. Por ejemplo:

```javascript
var nombre = "Juan";
let edad = 25;
const PI = 3.1416;
```


2. *Tipos de datos*: En JavaScript, existen diferentes tipos de datos, como números, cadenas de texto, booleanos, arreglos y objetos. Es importante comprender cómo se utilizan y manipulan estos tipos de datos en JavaScript.

3. *Operadores: Los operadores nos permiten realizar operaciones matemáticas, concatenar cadenas de texto, comparar valores y más. Algunos operadores comunes en JavaScript incluyen `+`, `-`, `*`, `/`, `===`, `>`, `<`, entre otros.

4. *Estructuras de control*: Las estructuras de control nos permiten tomar decisiones y repetir bloques de código. En JavaScript, utilizamos las siguientes estructuras de control:

   - `if`/`else`: Permite ejecutar un bloque de código si se cumple una condición o ejecutar un bloque alternativo si no se cumple.
   - `switch`: Permite seleccionar diferentes bloques de código basados en múltiples casos de una expresión.
   - `for`: Nos permite repetir un bloque de código un número específico de veces.
   - `while`/`do-while`: Nos permite repetir un bloque de código mientras se cumpla una condición.

5. *Funciones*: Las funciones nos permiten agrupar bloques de código y reutilizarlos. Pueden tener parámetros y devolver un resultado. Por ejemplo:

```javascript
function saludar(nombre) {
  console.log("¡Hola, " + nombre + "!");
}

saludar("Juan"); // Imprime: ¡Hola, Juan!
```





# Ejercicio: Adivina el número

En esta ejercio, aprenderemos los conceptos básicos de JavaScript y cómo utilizarlos para crear el juego "Adivina el número". ¡Vamos a empezar!

## Conceptos a cubrir

1. Variables: Las variables nos permiten almacenar y manipular datos en JavaScript.

2. Generación de números aleatorios: Aprenderemos cómo generar números aleatorios en un rango específico utilizando la función `Math.random()` y operaciones matemáticas.

3. Entrada del usuario: Utilizaremos la función `prompt()` para solicitar información al usuario y `parseInt()` para convertir la entrada en un número entero.

4. Condicionales (if/else): Los condicionales nos permiten tomar decisiones basadas en condiciones. Utilizaremos `if` y `else` para verificar si la suposición del usuario es correcta.

5. Bucles (while): Utilizaremos el bucle `while` para permitir que el usuario siga adivinando hasta que adivine correctamente.

6. Comparaciones: Aprenderemos a utilizar operadores de comparación para evaluar si la suposición del usuario es mayor, menor o igual al número aleatorio.

7. Salida de resultados: Utilizaremos `console.log()` para imprimir mensajes y proporcionar retroalimentación al usuario.

## Ejercicio: Adivina el número

Aquí está el código del juego "Adivina el número" que crearemos juntos:

```javascript
// Generar un número aleatorio entre 1 y 10
var numeroAleatorio = Math.floor(Math.random() * 10) + 1;

// Pedir al usuario que adivine el número
var suposicion = parseInt(prompt("Adivina el número (entre 1 y 10):"));

// Comprobar si la suposición es correcta y proporcionar retroalimentación
while (suposicion !== numeroAleatorio) {
  if (suposicion < numeroAleatorio) {
    console.log("Demasiado bajo. Intenta de nuevo.");
  } else {
    console.log("Demasiado alto. Intenta de nuevo.");
  }
  suposicion = parseInt(prompt("Adivina el número (entre 1 y 10):"));
}

// La suposición es correcta
console.log("¡Felicitaciones! Adivinaste el número correctamente.");
```

¡Felicidades! Has completado el ejercicio "Adivina el número" en JavaScript. Puedes experimentar con el código y agregar características adicionales, como contar los intentos o establecer límites de intentos.

## ¡Tarea Adicional!

Como tarea adicional, te invito a que modifiques el código del juego "Adivina el número" para implementar un sistema de conteo de intentos y mensajes personalizados relacionados con el acto de adivinar. Aquí tienes algunos pasos que puedes seguir:

- Crea una variable llamada intentos e inicialízala en 0 antes del bucle while.
- Incrementa el valor de intentos en cada iteración del bucle, justo después de pedir al usuario que adivine el número.
- Después del bucle while, agrega un bloque if para mostrar mensajes personalizados según la cantidad de intentos.
  - Si intentos es igual a 1, muestra un mensaje como: "¡Increíble! Adivinaste el número en tu primer intento. Eres un adivinador nato.".
  - Si intentos es menor o igual a 5, muestra un mensaje como: "¡Felicitaciones! Adivinaste el número en [intentos] intentos. Tienes habilidades para adivinar.".
  - Si intentos es mayor que 5 y menor o igual a 10, muestra un mensaje como: "¡Bien hecho! Adivinaste el número en [intentos] intentos. Puedes mejorar tus habilidades de adivinación.".
  - Si intentos es mayor que 10, muestra un mensaje como: "Adivinaste el número en [intentos] intentos. Sigue practicando, ¡el siguiente desafío te espera!".
- Ejecuta el código y verifica si los mensajes se muestran correctamente según la cantidad de intentos.

### Nota:
Para incrementar el valor de una variable en JavaScript, podemos utilizar el operador de incremento ++. Por ejemplo:

```javascript
var variable = 0;
variable++; // variable es igual a 1
variable++; // variable es igual a 2
```

También podemos utilizar el operador += para incrementar el valor de una variable. Por ejemplo:

```javascript
var variable = 0;
variable += 1; // variable es igual a 1
variable += 1; // variable es igual a 2
```

o simplemente sobreescribir el valor de la variable. Por ejemplo:

```javascript
var variable = 0;
variable = variable + 1; // variable es igual a 1
variable = variable + 1; // variable es igual a 2
```

Recuerda que puedes experimentar y agregar tus propios mensajes personalizados relacionados con el acto de adivinar. ¡Diviértete programando y sigue practicando tus habilidades en JavaScript!
No dudes en consultar si tienes alguna pregunta adicional. ¡Buena suerte!
