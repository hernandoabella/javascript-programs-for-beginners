# javascript-programs-for-beginnersEsta es una lista de programas de JavaScript para que los principiantes puedan subir de nivel rapidamente.

**1. Programa en JavaScript para Imprimir Hola Mundo:**

```jsx
console.log("¡Hola, Mundo!");
```

**2. Programa en JavaScript para Sumar Dos Números:**

```jsx
const num1 = 5;
const num2 = 10;
const suma = num1 + num2;
console.log("Suma:", suma);
```

**3. Programa en JavaScript para Encontrar la Raíz Cuadrada:**

```jsx
const numero = 25;
const raizCuadrada = Math.sqrt(numero);
console.log("Raíz cuadrada:", raizCuadrada);

```

**4. Programa en JavaScript para Calcular el Área de un Triángulo:**

```jsx
const base = 5;
const altura = 8;
const area = 0.5 * base * altura;
console.log("Área del triángulo:", area);
```

**5. Programa en JavaScript para Intercambiar Dos Variables:**

```jsx
let a = 5;
let b = 10;

console.log("Antes del intercambio: a =", a, "b =", b);

let temp = a;
a = b;
b = temp;

console.log("Después del intercambio: a =", a, "b =", b);
```

**6. Programa en JavaScript para Resolver una Ecuación Cuadrática:**

```jsx
const a = 2;
const b = -7;
const c = 3;

const discriminante = b * b - 4 * a * c;
const raiz1 = (-b + Math.sqrt(discriminante)) / (2 * a);
const raiz2 = (-b - Math.sqrt(discriminante)) / (2 * a);

console.log("Raíz 1:", raiz1);
console.log("Raíz 2:", raiz2);
```

**7. Programa en JavaScript para Convertir Kilómetros a Millas:**

```jsx
const kilometros = 10;
const millas = kilometros * 0.621371;
console.log(kilometros + " kilómetros =", millas + " millas");
```

**8. Programa en JavaScript para Convertir Grados Celsius a Fahrenheit:**

```jsx
const celsius = 30;
const fahrenheit = (celsius * 9/5) + 32;
console.log(celsius + "°C =", fahrenheit + "°F");
```

**9. Programa en JavaScript para Generar un Número Aleatorio:**

```jsx
const numAleatorio = Math.random(); // Genera un número aleatorio entre 0 (inclusive) y 1 (exclusivo)
console.log("Número aleatorio:", numAleatorio);
```

**10. Programa en JavaScript para Verificar si un número es Positivo, Negativo o Cero:**

```jsx
const numero = 5;

if (numero > 0) {
    console.log("El número es positivo");
} else if (numero < 0) {
    console.log("El número es negativo");
} else {
    console.log("El número es cero");
}
```

11. **Programa en JavaScript para Verificar si un Número es Par o Impar:**

```jsx
const numero = 10;

if (numero % 2 === 0) {
    console.log("El número es par");
} else {
    console.log("El número es impar");
}
```

12**. Programa en JavaScript para Encontrar el Mayor entre Tres Números:**

```jsx
const num1 = 5;
const num2 = 10;
const num3 = 8;

let mayor = num1;

if (num2 > mayor) {
    mayor = num2;
}
if (num3 > mayor) {
    mayor = num3;
}

console.log("El número mayor es:", mayor);
```

13**. Programa en JavaScript para Verificar si un Número es Primo:**

```jsx
const numero = 7;
let esPrimo = true;

if (numero === 1) {
    esPrimo = false;
} else {
    for (let i = 2; i <= Math.sqrt(numero); i++) {
        if (numero % i === 0) {
            esPrimo = false;
            break;
        }
    }
}

if (esPrimo) {
    console.log("El número es primo");
} else {
    console.log("El número no es primo");
}
```

14**. Programa en JavaScript para Imprimir Todos los Números Primos en un Intervalo:**

```jsx
const inicio = 10;
const fin = 50;

for (let numero = inicio; numero <= fin; numero++) {
    let esPrimo = true;

    if (numero === 1) {
        esPrimo = false;
    } else {
        for (let i = 2; i <= Math.sqrt(numero); i++) {
            if (numero % i === 0) {
                esPrimo = false;
                break;
            }
        }
    }

    if (esPrimo) {
        console.log(numero);
    }
}
```

15**. Programa en JavaScript para Encontrar el Factorial de un Número:**

```jsx
const numero = 5;
let factorial = 1;

for (let i = 1; i <= numero; i++) {
    factorial *= i;
}

console.log("El factorial de", numero, "es:", factorial);
```

16**. Programa en JavaScript para Mostrar la Tabla de Multiplicar:**

```jsx
const numero = 7;

for (let i = 1; i <= 10; i++) {
    console.log(numero + " x " + i + " =", numero * i);
}
```

17. **Programa en JavaScript para Imprimir la Secuencia de Fibonacci:**

```jsx
const n = 10;
let a = 0, b = 1;

console.log("Secuencia de Fibonacci:");

for (let i = 1; i <= n; i++) {
    console.log(a);
    const temp = a + b;
    a = b;
    b = temp;
}
```

1. **Programa en JavaScript para Verificar si un Número es un Número Armstrong:**

```jsx
const numero = 153;
let numOriginal = numero;
let suma = 0;

while (numOriginal > 0) {
    const digito = numOriginal % 10;
    suma += digito ** 3;
    numOriginal = Math.floor(numOriginal / 10);
}

if (suma === numero) {
    console.log("El número es un número Armstrong");
} else {
    console.log("El número no es un número Armstrong");
}
```

19**. Programa en JavaScript para Encontrar los Números Armstrong en un Intervalo:**

```jsx
const inicio = 100;
const fin = 1000;

console.log("Números Armstrong en el intervalo", inicio, "a", fin + ":");

for (let numero = inicio; numero <= fin; numero++) {
    let numOriginal = numero;
    let suma = 0;
    const n = String(numero).length;

    while (numOriginal > 0) {
        const digito = numOriginal % 10;
        suma += digito ** n;
        numOriginal = Math.floor(numOriginal / 10);
    }

    if (suma === numero) {
        console.log(numero);
    }
}
```

20**. Programa en JavaScript para Crear una Calculadora Simple:**

```jsx
const num1 = parseFloat(prompt("Ingresa el primer número:"));
const num2 = parseFloat(prompt("Ingresa el segundo número:"));
const operacion = prompt("Ingresa la operación (+, -, *, /):");

let resultado;

switch (operacion) {
    case "+":
        resultado = num1 + num2;
        break;
    case "-":
        resultado = num1 - num2;
        break;
    case "*":
        resultado = num1 * num2;
        break;
    case "/":
        resultado = num1 / num2;
        break;
    default:
        console.log("Operación no válida");
}

console.log("Resultado:", resultado);
```

**21. Programa en JavaScript para Encontrar la Suma de Números Naturales:**

```jsx
const n = parseInt(prompt("Ingresa un número natural:"));
let suma = 0;

for (let i = 1; i <= n; i++) {
    suma += i;
}

console.log("La suma de los primeros", n, "números naturales es:", suma);
```

22**. Programa en JavaScript para Verificar si los Números Tienen el Mismo Último Dígito:**

```jsx
const num1 = parseInt(prompt("Ingresa el primer número:"));
const num2 = parseInt(prompt("Ingresa el segundo número:"));

const ultimoDigito1 = num1 % 10;
const ultimoDigito2 = num2 % 10;

if (ultimoDigito1 === ultimoDigito2) {
    console.log("Los números tienen el mismo último dígito");
} else {
    console.log("Los números no tienen el mismo último dígito");
}
```

23**. Programa en JavaScript para Encontrar el MCD o MCM:**

```jsx
const num1 = parseInt(prompt("Ingresa el primer número:"));
const num2 = parseInt(prompt("Ingresa el segundo número:"));

let mcd, a, b;
a = num1;
b = num2;

while (b !== 0) {
    const temp = b;
    b = a % b;
    a = temp;
}

mcd = a;
const mcm = (num1 * num2) / mcd;

console.log("MCD:", mcd);
console.log("MCM:", mcm);
```

24**. Programa en JavaScript para Encontrar el MCM:**

```jsx
const num1 = parseInt(prompt("Ingresa el primer número:"));
const num2 = parseInt(prompt("Ingresa el segundo número:"));

let mcm;

for (let i = Math.max(num1, num2); ; i++) {
    if (i % num1 === 0 && i % num2 === 0) {
        mcm = i;
        break;
    }
}

console.log("MCM:", mcm);
```

25**. Programa en JavaScript para Encontrar los Factores de un Número:**

```jsx
const numero = parseInt(prompt("Ingresa un número:"));

console.log("Factores de", numero + ":");

for (let i = 1; i <= numero; i++) {
    if (numero % i === 0) {
        console.log(i);
    }
}
```

26**. Programa en JavaScript para Encontrar la Suma de Números Naturales Usando Recursión:**

```jsx
function sumaNaturales(n) {
    if (n === 1) {
        return 1;
    } else {
        return n + sumaNaturales(n - 1);
    }
}

const num = parseInt(prompt("Ingresa un número natural:"));
const suma = sumaNaturales(num);

console.log("La suma de los primeros", num, "números naturales es:", suma);
```

27**. Programa en JavaScript para Adivinar un Número Aleatorio:**

```jsx
const numeroAleatorio = Math.floor(Math.random() * 100) + 1;
let intentos = 0;
let intentoUsuario;

do {
    intentoUsuario = parseInt(prompt("Adivina el número (entre 1 y 100):"));
    intentos++;

    if (intentoUsuario < numeroAleatorio) {
        console.log("El número es mayor");
    } else if (intentoUsuario > numeroAleatorio) {
        console.log("El número es menor");
    } else {
        console.log("¡Correcto! Adivinaste el número en", intentos, "intentos.");
    }
} while (intentoUsuario !== numeroAleatorio);
```

28**. Programa en JavaScript para Mezclar una Baraja de Cartas:**

```jsx
const valores = ["2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K", "A"];
const palos = ["Corazones", "Diamantes", "Tréboles", "Picas"];
const baraja = [];

for (const palo of palos) {
    for (const valor of valores) {
        baraja.push(`${valor} de ${palo}`);
    }
}

console.log("Baraja de cartas mezclada:", baraja);
```

29**. Programa en JavaScript para Mostrar la Secuencia de Fibonacci Usando Recursión:**

```jsx
function fibonacci(n) {
    if (n <= 1) {
        return n;
    } else {
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
}

const num = parseInt(prompt("Ingresa un número para generar la secuencia de Fibonacci:"));

console.log("Secuencia de Fibonacci:");

for (let i = 0; i < num; i++) {
    console.log(fibonacci(i));
}
```

30**. Programa en JavaScript para Encontrar el Factorial de un Número Usando Recursión:**

```jsx
function factorial(n) {
    if (n === 0 || n === 1) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}

const num = parseInt(prompt("Ingresa un número para encontrar su factorial:"));
const resultado = factorial(num);

console.log("Factorial de", num, "es:", resultado);
```

31**. Programa en JavaScript para Convertir un Número Decimal a Binario:**

```jsx
const decimal = parseInt(prompt("Ingresa un número decimal:"));
const binario = decimal.toString(2);

console.log("Número decimal", decimal, "en binario:", binario);
```

32**. Programa en JavaScript para Encontrar el Valor ASCII de un Carácter:**

```jsx
const caracter = prompt("Ingresa un carácter:");
const codigoAscii = caracter.charCodeAt(0);

console.log("El valor ASCII de", caracter, "es:", codigoAscii);
```

33**. Programa en JavaScript para Verificar si una Cadena es Palíndromo o No:**

```jsx
function esPalindromo(cadena) {
    const cadenaLimpia = cadena.toLowerCase().replace(/[^a-z0-9]/g, "");
    const cadenaReversa = cadenaLimpia.split("").reverse().join("");
    return cadenaLimpia === cadenaReversa;
}

const palabra = prompt("Ingresa una palabra o frase para verificar si es un palíndromo:");
const esPalin = esPalindromo(palabra);

if (esPalin) {
    console.log("La cadena es un palíndromo.");
} else {
    console.log("La cadena no es un palíndromo.");
}
```

34**. Programa en JavaScript para Ordenar Palabras en Orden Alfabético:**

```jsx
const palabras = prompt("Ingresa una lista de palabras separadas por comas:").split(",");
palabras.sort();
console.log("Palabras ordenadas:", palabras);
```

35**. Programa en JavaScript para Reemplazar Caracteres en una Cadena:**

```jsx
const cadena = "Hola, mundo!";
const nuevaCadena = cadena.replace("Hola", "Adiós");
console.log("Cadena original:", cadena);
console.log("Nueva cadena:", nuevaCadena);
```

**36. Programa en JavaScript para Invertir una Cadena:**

```jsx
const cadena = "JavaScript";
const cadenaInvertida = cadena.split("").reverse().join("");
console.log("Cadena original:", cadena);
console.log("Cadena invertida:", cadenaInvertida);
```

37**. Programa en JavaScript para Crear Objetos de Diferentes Formas:**

```jsx
// Forma 1: Objeto Literal
const persona1 = {
    nombre: "Juan",
    edad: 30,
    profesion: "Ingeniero"
};

// Forma 2: Constructor de Objeto
function Persona(nombre, edad, profesion) {
    this.nombre = nombre;
    this.edad = edad;
    this.profesion = profesion;
}
const persona2 = new Persona("María", 28, "Doctora");

// Forma 3: Clases (ES6)
class Persona {
    constructor(nombre, edad, profesion) {
        this.nombre = nombre;
        this.edad = edad;
        this.profesion = profesion;
    }
}
const persona3 = new Persona("Carlos", 25, "Abogado");
```

38**. Programa en JavaScript para Verificar el Número de Ocurrencias de un Carácter en una Cadena:**

```jsx
const cadena = "programación";
const caracter = "a";
const conteo = cadena.split(caracter).length - 1;
console.log("Número de ocurrencias de", caracter, ":", conteo);
```

39**. Programa en JavaScript para Convertir la Primera Letra de una Cadena en Mayúscula:**

```jsx
const palabra = "javascript";
const primeraLetraMayuscula = palabra.charAt(0).toUpperCase() + palabra.slice(1);
console.log("Palabra original:", palabra);
console.log("Palabra con la primera letra en mayúscula:", primeraLetraMayuscula);
```

40**. Programa en JavaScript para Contar el Número de Vocales en una Cadena:**

```jsx
const cadena = "elefante";
const vocales = cadena.match(/[aeiou]/gi);
const numeroVocales = vocales ? vocales.length : 0;
console.log("Número de vocales en", cadena + ":", numeroVocales);
```

41**. Programa en JavaScript para Eliminar una Propiedad de un Objeto:**

```jsx
const persona = {
    nombre: "Ana",
    edad: 28,
    profesion: "Diseñadora"
};

delete persona.edad;
console.log("Objeto después de eliminar la propiedad 'edad':", persona);
```

1. **Programa en JavaScript para Verificar si una Cadena Empieza y Termina con Ciertos Caracteres:**

```jsx
const cadena = "Hola, mundo!";
const empiezaCon = "Hola";
const terminaCon = "!";

const empiezaCorrecto = cadena.startsWith(empiezaCon);
const terminaCorrecto = cadena.endsWith(terminaCon);

console.log("La cadena empieza con", empiezaCon + ":", empiezaCorrecto);
console.log("La cadena termina con", terminaCon + ":", terminaCorrecto);
```

43**. Programa en JavaScript para Verificar si una Clave Existe en un Objeto:**

```jsx
const persona = {
    nombre: "Luis",
    edad: 32,
    profesion: "Instructor"
};

const clave = "nombre";
if (clave in persona) {
    console.log("La clave", clave, "existe en el objeto");
} else {
    console.log("La clave", clave, "no existe en el objeto");
}
```

44**. Programa en JavaScript para Clonar un Objeto:**

```jsx
const objetoOriginal = {
    propiedad1: "valor1",
    propiedad2: "valor2"
};

const objetoClonado = {...objetoOriginal};
console.log("Objeto original:", objetoOriginal);
console.log("Objeto clonado:", objetoClonado);
```

45**. Programa en JavaScript para Recorrer un Objeto:**

```jsx
const persona = {
    nombre: "Laura",
    edad: 25,
    profesion: "Arquitecta"
};

console.log("Propiedades del objeto persona:");
for (const propiedad in persona) {
    console.log(propiedad + ":", persona[propiedad]);
}
```

46**. Programa en JavaScript para Combinar Propiedades de Dos Objetos:**

```jsx
const objeto1 = { a: 1, b: 2 };
const objeto2 = { b: 3, c: 4 };

const objetoCombinado = { ...objeto1, ...objeto2 };
console.log("Objeto combinado:", objetoCombinado);
```

47**. Programa en JavaScript para Contar el Número de Claves/Propiedades en un Objeto:**

```jsx
const objeto = { a: 1, b: 2, c: 3 };

const numeroClaves = Object.keys(objeto).length;
console.log("Número de claves en el objeto:", numeroClaves);
```

48**. Programa en JavaScript para Agregar un Par Clave/Valor a un Objeto:**

```jsx
const persona = { nombre: "María", edad: 30 };

persona.profesion = "Ingeniera";
console.log("Objeto después de agregar una propiedad:", persona);
```

**49. Programa en JavaScript para Reemplazar Todas las Ocurrencias de una Cadena:**

```jsx
const cadena = "Hola, mundo! Hola, universo!";
const nuevaCadena = cadena.replace(/Hola/g, "Adiós");
console.log("Cadena original:", cadena);
console.log("Nueva cadena:", nuevaCadena);
```

**50. Programa en JavaScript para Crear Cadenas Multilínea:**

```jsx
const multilinea = `Esta es una cadena
que ocupa múltiples líneas
en el código.`;

console.log(multilinea);
```

**51. Programa en JavaScript para Formatear Números como Cadenas de Moneda:**

```jsx
const precio = 1500.75;
const precioFormateado = precio.toLocaleString("es-ES", { style: "currency", currency: "EUR" });
console.log("Precio formateado:", precioFormateado);
```

**52. Programa en JavaScript para Generar una Cadena Aleatoria:**

```jsx
function generarCadenaAleatoria(longitud) {
    const caracteres = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789";
    let cadena = "";

    for (let i = 0; i < longitud; i++) {
        const indice = Math.floor(Math.random() * caracteres.length);
        cadena += caracteres.charAt(indice);
    }

    return cadena;
}

const cadenaAleatoria = generarCadenaAleatoria(10);
console.log("Cadena aleatoria:", cadenaAleatoria);
```

**53. Programa en JavaScript para Verificar si una Cadena Comienza con Otra Cadena:**

```jsx
const cadena = "JavaScript es genial!";
const comienzaCon = "JavaScript";

const comienzaCorrecto = cadena.startsWith(comienzaCon);
console.log("La cadena comienza con", comienzaCon + ":", comienzaCorrecto);
```

**54. Programa en JavaScript para Recortar una Cadena:**

```jsx
const cadena = "    ¡Hola, mundo!    ";
const cadenaRecortada = cadena.trim();
console.log("Cadena original:", cadena);
console.log("Cadena recortada:", cadenaRecortada);
```

**55. Programa en JavaScript para Convertir Objetos a Cadenas:**

```jsx
const objeto = { a: 1, b: 2, c: 3 };
const cadena = JSON.stringify(objeto);

console.log("Objeto:", objeto);
console.log("Cadena:", cadena);
```

**56. Programa en JavaScript para Verificar si una Cadena Contiene una Subcadena:**

```jsx
const cadena = "JavaScript es genial!";
const subcadena = "genial";

const contieneSubcadena = cadena.includes(subcadena);
console.log("La cadena contiene la subcadena", subcadena + ":", contieneSubcadena);
```

**57. Programa en JavaScript para Comparar Dos Cadenas:**

```jsx
const cadena1 = "Hola";
const cadena2 = "hola";

if (cadena1 === cadena2) {
    console.log("Las cadenas son iguales");
} else {
    console.log("Las cadenas son diferentes");
}
```

1. **Programa en JavaScript para Codificar una Cadena en Base64:**

```jsx
const cadena = "Hola, mundo!";
const cadenaCodificada = btoa(cadena);
console.log("Cadena original:", cadena);
console.log("Cadena codificada:", cadenaCodificada);
```

**59. Programa en JavaScript para Reemplazar Todas las Instancias de un Carácter en una Cadena:**

```jsx
const cadena = "javascript";
const caracterOriginal = "a";
const caracterNuevo = "A";

const nuevaCadena = cadena.replace(new RegExp(caracterOriginal, "g"), caracterNuevo);
console.log("Cadena original:", cadena);
console.log("Nueva cadena:", nuevaCadena);
```

**60. Programa en JavaScript para Calcular el Área de un Triángulo:**

```jsx
const base = 5;
const altura = 8;
const area = 0.5 * base * altura;
console.log("Área del triángulo:", area);
```

**61. Programa en JavaScript para Reemplazar Todos los Saltos de Línea con `<br>`:**

```jsx
const textoConSaltos = "Línea 1\nLínea 2\nLínea 3";
const textoConBR = textoConSaltos.replace(/\n/g, "<br>");

console.log("Texto con saltos de línea:", textoConSaltos);
console.log("Texto con <br>:", textoConBR);
```

**62. Programa en JavaScript para Mostrar la Fecha y la Hora:**

```jsx
const fechaActual = new Date();
const opciones = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric', hour: 'numeric', minute: 'numeric', second: 'numeric', timeZoneName: 'short' };
const fechaYHora = fechaActual.toLocaleDateString('es-ES', opciones);

console.log("Fecha y hora actual:", fechaYHora);
```

**63. Programa en JavaScript para Verificar si un Año es Bisiesto:**

```jsx
function esBisiesto(año) {
    return (año % 4 === 0 && año % 100 !== 0) || (año % 400 === 0);
}

const año = parseInt(prompt("Ingresa un año:"));
if (esBisiesto(año)) {
    console.log(año + " es un año bisiesto.");
} else {
    console.log(año + " no es un año bisiesto.");
}
```

**64. Programa en JavaScript para Formatear la Fecha:**

```jsx
const fecha = new Date();
const opciones = { weekday: "long", year: "numeric", month: "long", day: "numeric" };
const fechaFormateada = fecha.toLocaleDateString("es-ES", opciones);
console.log("Fecha formateada:", fechaFormateada);
```

**65. Programa en JavaScript para Mostrar la Fecha Actual:**

```jsx
const fechaActual = new Date();
console.log("Fecha actual:", fechaActual.toDateString());
```

**66. Programa en JavaScript para Comparar el Valor de Dos Fechas:**

```jsx
const fecha1 = new Date("2023-08-25");
const fecha2 = new Date("2023-08-20");

if (fecha1 > fecha2) {
    console.log("La fecha 1 es posterior a la fecha 2.");
} else if (fecha1 < fecha2) {
    console.log("La fecha 1 es anterior a la fecha 2.");
} else {
    console.log("Las fechas son iguales.");
}
```

**67.** **Programa en JavaScript para Crear una Temporizador de Cuenta Regresiva:**

```jsx
function countdownTimer(tiempo) {
    const intervalo = setInterval(function() {
        console.log(tiempo);
        tiempo--;

        if (tiempo < 0) {
            clearInterval(intervalo);
            console.log("¡Tiempo terminado!");
        }
    }, 1000);
}

const segundos = parseInt(prompt("Ingresa la cantidad de segundos para la cuenta regresiva:"));
countdownTimer(segundos);
```

**68. Programa en JavaScript para Eliminar un Elemento Específico de un Array:**

```jsx
const numeros = [1, 2, 3, 4, 5];
const elementoEliminar = 3;

const indice = numeros.indexOf(elementoEliminar);
if (indice !== -1) {
    numeros.splice(indice, 1);
}

console.log("Array después de eliminar el elemento:", numeros);
```

**69. Programa en JavaScript para Verificar si un Array Contiene un Valor Especificado:**

```jsx
const numeros = [1, 2, 3, 4, 5];
const valorBuscado = 3;

const contieneValor = numeros.includes(valorBuscado);
if (contieneValor) {
    console.log("El array contiene el valor", valorBuscado);
} else {
    console.log("El array no contiene el valor", valorBuscado);
}
```

**70. Programa en JavaScript para Insertar un Elemento en un Array:**

```jsx
const numeros = [1, 2, 3, 5];
const elementoInsertar = 4;
const indice = 3;

numeros.splice(indice, 0, elementoInsertar);
console.log("Array después de insertar el elemento:", numeros);
```

**71. Programa en JavaScript para Agregar un Objeto al Final de un Array:**

```jsx
const personas = [
    { nombre: "Juan", edad: 30 },
    { nombre: "María", edad: 25 }
];

const nuevaPersona = { nombre: "Carlos", edad: 28 };
personas.push(nuevaPersona);
console.log("Array después de agregar el objeto:", personas);
```

**72. Programa en JavaScript para Verificar si un Objeto es un Array:**

```jsx
const arreglo = [1, 2, 3];
const objeto = { a: 1, b: 2 };

if (Array.isArray(arreglo)) {
    console.log("El objeto es un array.");
} else {
    console.log("El objeto no es un array.");
}

if (Array.isArray(objeto)) {
    console.log("El objeto es un array.");
} else {
    console.log("El objeto no es un array.");
}
```

**73. Programa en JavaScript para Vaciar un Array:**

```jsx
const numeros = [1, 2, 3, 4, 5];
numeros.length = 0;
console.log("Array vaciado:", numeros);
```

**74. Programa en JavaScript para Agregar un Elemento al Inicio de un Array:**

```jsx
const numeros = [2, 3, 4, 5];
const elementoAgregar = 1;

numeros.unshift(elementoAgregar);
console.log("Array después de agregar el elemento:", numeros);
```

**75. Programa en JavaScript para Eliminar Duplicados de un Array:**

```jsx
const numeros = [1, 2, 2, 3, 4, 4, 5];
const numerosUnicos = [...new Set(numeros)];

console.log("Array original:", numeros);
console.log("Array sin duplicados:", numerosUnicos);
```

**76. Programa en JavaScript para Combinar Dos Arrays y Eliminar Elementos Duplicados:**

```jsx
const array1 = [1, 2, 3];
const array2 = [3, 4, 5];
const arrayCombinado = [...new Set([...array1, ...array2])];

console.log("Array 1:", array1);
console.log("Array 2:", array2);
console.log("Array combinado sin duplicados:", arrayCombinado);
```

**77. Programa en JavaScript para Ordenar un Array de Objetos por Valores de Propiedades:**

```jsx
const personas = [
    { nombre: "Juan", edad: 30 },
    { nombre: "María", edad: 25 },
    { nombre: "Carlos", edad: 28 }
];

personas.sort((a, b) => a.edad - b.edad);
console.log("Array de personas ordenado por edad:", personas);
```

**78. Programa en JavaScript para Crear un Array Bidimensional:**

```jsx
const matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

console.log("Matriz:", matriz);
```

**79. Programa en JavaScript para Extraer Valores de Propiedades Dadas de Objetos como Array:**

```jsx
const personas = [
    { nombre: "Juan", edad: 30 },
    { nombre: "María", edad: 25 },
    { nombre: "Carlos", edad: 28 }
];

const edades = personas.map(persona => persona.edad);
console.log("Array de edades:", edades);
```

**80. Programa en JavaScript para Comparar Elementos de Dos Arrays:**

```jsx
const array1 = [1, 2, 3];
const array2 = [2, 3, 4];

const sonIguales = JSON.stringify(array1) === JSON.stringify(array2);
console.log("Los arrays son iguales:", sonIguales);
```

**81. Programa en JavaScript para Obtener un Elemento Aleatorio de un Array:**

```jsx
function obtenerElementoAleatorio(array) {
    const indiceAleatorio = Math.floor(Math.random() * array.length);
    return array[indiceAleatorio];
}

const colores = ["rojo", "verde", "azul", "amarillo"];
const colorAleatorio = obtenerElementoAleatorio(colores);
console.log("Color aleatorio:", colorAleatorio);
```

**82. Programa en JavaScript para Realizar la Intersección Entre Dos Arrays:**

```jsx
function interseccionArrays(array1, array2) {
    return array1.filter(valor => array2.includes(valor));
}

const array1 = [1, 2, 3, 4, 5];
const array2 = [3, 4, 5, 6, 7];
const interseccion = interseccionArrays(array1, array2);
console.log("Intersección:", interseccion);
```

**83. Programa en JavaScript para Dividir un Array en Segmentos Más Pequeños:**

```jsx
function dividirArray(array, tamaño) {
    const segmentos = [];
    for (let i = 0; i < array.length; i += tamaño) {
        segmentos.push(array.slice(i, i + tamaño));
    }
    return segmentos;
}

const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9];
const segmentos = dividirArray(numeros, 3);
console.log("Segmentos:", segmentos);
```

**84. Programa en JavaScript para Incluir un Archivo JS en Otro Archivo JS:**

```jsx
// Archivo: archivo1.js
console.log("Este es el archivo 1.");

// Archivo: archivo2.js
console.log("Este es el archivo 2.");
```

**85. Programa en JavaScript para Obtener la Extensión de un Archivo:**

```jsx
const archivo = "documento.pdf";
const extension = archivo.slice(archivo.lastIndexOf(".") + 1);
console.log("Extensión del archivo:", extension);
```

**86. Programa en JavaScript para Verificar si una Variable es indefinida o nula:**

```jsx
function verificarUndefinedNull(variable) {
    if (variable === undefined) {
        console.log("La variable es undefined.");
    } else if (variable === null) {
        console.log("La variable es null.");
    } else {
        console.log("La variable no es undefined ni null.");
    }
}

let variable1;
const variable2 = null;
const variable3 = "Hola";

verificarUndefinedNull(variable1);
verificarUndefinedNull(variable2);
verificarUndefinedNull(variable3);
```

**87. Programa en JavaScript para Establecer un Valor de Parámetro Predeterminado para una Función:**

```jsx
function saludar(nombre = "Usuario") {
    console.log("¡Hola, " + nombre + "!");
}

saludar(); // Salida: ¡Hola, Usuario!
saludar("Juan"); // Salida: ¡Hola, Juan!
```

**88. Programa en JavaScript para Ilustrar Diferentes Operaciones de Conjuntos:**

```jsx
const conjuntoA = new Set([1, 2, 3]);
const conjuntoB = new Set([3, 4, 5]);

const union = new Set([...conjuntoA, ...conjuntoB]);
const interseccion = new Set([...conjuntoA].filter(x => conjuntoB.has(x)));
const diferencia = new Set([...conjuntoA].filter(x => !conjuntoB.has(x)));

console.log("Unión:", union);
console.log("Intersección:", interseccion);
console.log("Diferencia:", diferencia);
```

**89. Programa en JavaScript para Generar un Número Aleatorio Entre Dos Números:**

```jsx
function numeroAleatorio(min, max) {
    return Math.floor(Math.random() * (max - min + 1)) + min;
}

const numeroAleatorio = numeroAleatorio(1, 100);
console.log("Número aleatorio:", numeroAleatorio);
```

**90. Programa en JavaScript para Obtener la URL Actual:**

```jsx
const urlActual = window.location.href;
console.log("URL actual:", urlActual);
```

**91. Programa en JavaScript para Validar una Dirección de Correo Electrónico:**

```jsx
function validarCorreo(correo) {
    const patron = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;
    return patron.test(correo);
}

const correo = "usuario@example.com";
if (validarCorreo(correo)) {
    console.log("La dirección de correo es válida.");
} else {
    console.log("La dirección de correo no es válida.");
}
```

**92. Programa en JavaScript para Verificar si una Variable es de Tipo Función:**

```jsx
const funcionEjemplo = function() {
    console.log("Esta es una función de ejemplo.");
};

if (typeof funcionEjemplo === "function") {
    console.log("La variable es de tipo función.");
} else {
    console.log("La variable no es de tipo función.");
}
```

**93. Programa en JavaScript para Trabajar con Constantes:**

```jsx
const PI = 3.14159;
const URL_API = "https://api.example.com";
console.log("Valor de PI:", PI);
console.log("URL de la API:", URL_API);
```

**94. Programa en JavaScript para Pasar un Parámetro a una Función setTimeout():**

```jsx
function mostrarMensaje(mensaje) {
    console.log(mensaje);
}

setTimeout(mostrarMensaje, 2000, "¡Este es un mensaje después de 2 segundos!");
```

**95. Programa en JavaScript para Generar un Rango de Números y Caracteres:**

```jsx
function generarRango(inicio, fin) {
    const rango = [];
    for (let i = inicio; i <= fin; i++) {
        rango.push(i);
    }
    return rango;
}

const rangoNumeros = generarRango(1, 10);
console.log("Rango de números:", rangoNumeros);

const rangoCaracteres = generarRango("A", "F");
console.log("Rango de caracteres:", rangoCaracteres);
```

**96. Programa en JavaScript para Realizar Sobrecarga de Funciones:**

```jsx
function suma(a, b) {
    return a + b;
}

function suma(a, b, c) {
    return a + b + c;
}

console.log(suma(1, 2)); // Salida: NaN
console.log(suma(1, 2, 3)); // Salida: 6
```

**97. Programa en JavaScript para Implementar una Pila:**

```jsx
class Pila {
    constructor() {
        this.items = [];
    }

    push(elemento) {
        this.items.push(elemento);
    }

    pop() {
        return this.items.pop();
    }

    peek() {
        return this.items[this.items.length - 1];
    }

    estaVacia() {
        return this.items.length === 0;
    }

    tamano() {
        return this.items.length;
    }
}

const pila = new Pila();
pila.push(1);
pila.push(2);
pila.push(3);

console.log("Elemento superior:", pila.peek()); // Salida: 3
console.log("Tamaño de la pila:", pila.tamano()); // Salida: 3
```

**98. Programa en JavaScript para Implementar una Cola:**

```jsx
class Cola {
    constructor() {
        this.items = [];
    }

    encolar(elemento) {
        this.items.push(elemento);
    }

    desencolar() {
        return this.items.shift();
    }

    frente() {
        return this.items[0];
    }

    estaVacia() {
        return this.items.length === 0;
    }

    tamano() {
        return this.items.length;
    }
}

const cola = new Cola();
cola.encolar(1);
cola.encolar(2);
cola.encolar(3);

console.log("Elemento frontal:", cola.frente()); // Salida: 1
console.log("Tamaño de la cola:", cola.tamano()); // Salida: 3
```

**99. Programa en JavaScript para Verificar si un Número es Decimal o Entero:**

```jsx
function esDecimal(numero) {
    return numero % 1 !== 0;
}

const numeroDecimal = 3.14;
const numeroEntero = 7;

console.log(numeroDecimal + " es decimal:", esDecimal(numeroDecimal)); // Salida: true
console.log(numeroEntero + " es decimal:", esDecimal(numeroEntero)); // Salida: false
```

**100. Programa en JavaScript para Pasar una Función como Parámetro:**

```jsx
function ejecutarFuncion(funcion) {
    funcion();
}

function saludar() {
    console.log("¡Hola, mundo!");
}

ejecutarFuncion(saludar); // Salida: ¡Hola, mundo!
```

**101. Programa en JavaScript para Obtener las Dimensiones de una Imagen:**

```jsx
const imagen = new Image();
imagen.src = "imagen.jpg";

imagen.onload = function() {
    const ancho = imagen.width;
    const alto = imagen.height;
    console.log("Ancho de la imagen:", ancho);
    console.log("Alto de la imagen:", alto);
};
```

**102. Programa en JavaScript para Eliminar Todos los Espacios en Blanco de un Texto:**

```jsx
const textoConEspacios = "   Esto es un texto con espacios   ";
const textoSinEspacios = textoConEspacios.replace(/\s+/g, "");
console.log("Texto original:", textoConEspacios);
console.log("Texto sin espacios:", textoSinEspacios);
```

**103. Programa en JavaScript para Escribir en la Consola:**

```jsx
console.log("Este es un mensaje en la consola.");
```

**104. Programa en JavaScript para Convertir una Fecha a Número:**

```jsx
const fecha = new Date();
const numeroFecha = +fecha;
console.log("Fecha como número:", numeroFecha);
```
