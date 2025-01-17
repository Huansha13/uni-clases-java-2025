# Guía de Laboratorio Práctica: Estructuras de Programación

## Objetivo

Desarrollar programas que implementen estructuras de control condicionales y repetitivas, con un enfoque en la declaración y uso de variables, operadores, y la creación de un menú interactivo usando la estructura `switch`.

## Instrucciones

1. **Herramientas requeridas**: Un editor de código como Visual Studio Code, IntelliJ IDEA, o cualquier IDE que soporte el lenguaje de programación elegido (sugerido: Java o C++).
2. **Formato del archivo**: El programa final debe guardarse con el formato correspondiente (“.java” o “.cpp”).
3. **Lenguaje sugerido**: Puede adaptarse según las necesidades del grupo.

---

### Actividad 1: Declaración y uso de variables

**Instrucciones:**\
Crea un programa que declare las siguientes variables:

- Nombre del usuario (String)
- Edad (int)
- Saldo de una cuenta bancaria (double)
- Estado civil (boolean: `true` si está casado, `false` si no lo está)

Imprime los valores de cada una con el formato:

```
Nombre: [nombre]
Edad: [edad]
Saldo: [saldo]
Casado: [estado_civil]
```

---

### Actividad 2: Operadores aritméticos, relacionales y lógicos

**Instrucciones:**\
Escribe un programa que realice las siguientes operaciones:

1. Solicita dos números al usuario.
2. Realiza las operaciones básicas: suma, resta, multiplicación, división.
3. Determina si el primer número es mayor que el segundo usando operadores relacionales.
4. Verifica si ambos números son positivos y mayores que 10 usando operadores lógicos.
5. Imprime los resultados de todas las operaciones.

Ejemplo de salida:

```
Suma: 15
Resta: 5
Multiplicación: 50
División: 2.5
Primer número > Segundo número: true
Ambos números son positivos y mayores que 10: false
```

---

### Actividad 3: Estructuras condicionales

**Instrucciones:**\
Desarrolla un programa que solicite al usuario su edad y realice las siguientes verificaciones:

1. Si la edad es menor de 18, imprimir: “Eres menor de edad.”
2. Si la edad está entre 18 y 65, imprimir: “Eres un adulto.”
3. Si la edad es mayor o igual a 65, imprimir: “Eres una persona de la tercera edad.”

---

### Actividad 4: Estructuras repetitivas

**Instrucciones:**\
Crea un programa que imprima los números del 1 al 10 utilizando las siguientes estructuras:

1. Un bucle `for`
2. Un bucle `while`
3. Un bucle `do-while`

El programa debe imprimir el mismo resultado tres veces, uno por cada tipo de bucle.

---

### Actividad 5: Creación de un menú interactivo usando `switch`

**Instrucciones:**\
Crea un programa que despliegue un menú con las siguientes opciones:

```
1. Calcular el cuadrado de un número
2. Determinar si un número es par o impar
3. Salir
```

1. Solicita al usuario que elija una opción del menú.
2. Si elige la opción 1, solicita un número y calcula su cuadrado.
3. Si elige la opción 2, solicita un número y determina si es par o impar.
4. Si elige la opción 3, termina el programa.
5. El menú debe repetirse hasta que el usuario elija la opción de salir.

Ejemplo de salida:

```
Menú:
1. Calcular el cuadrado de un número
2. Determinar si un número es par o impar
3. Salir
Seleccione una opción: 1
Ingrese un número: 4
El cuadrado de 4 es 16.
```
