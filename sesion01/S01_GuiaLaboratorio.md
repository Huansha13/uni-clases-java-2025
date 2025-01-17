# Introducción a Java

## Objetivo
Desarrollar habilidades prácticas en la programación en Java mediante la creación de programas que implementen los conceptos básicos del lenguaje: características del lenguaje orientado a objetos, estructura de un programa y tipos de datos.

---

## Actividades Prácticas

### Actividad 1: Hola Mundo en Java
**Objetivo:** Familiarizarse con la estructura básica de un programa en Java.

**Instrucciones:**
1. Crea un proyecto nuevo llamado `IntroduccionJava`.
2. Dentro del proyecto, crea una clase llamada `HolaMundo`.
3. Escribe el siguiente código:

```java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("¡Hola, Mundo!");
    }
}
```

4. Ejecuta el programa y verifica que se imprima el mensaje en la consola.

**Resultado Esperado:** El mensaje "¡Hola, Mundo!" aparece en la consola.

---

### Actividad 2: Características del Lenguaje Orientado a Objetos
**Objetivo:** Implementar clases y objetos básicos.

**Instrucciones:**
1. Crea una clase llamada `Persona` con los siguientes atributos:
   - `nombre` (tipo `String`)
   - `edad` (tipo `int`)
2. Agrega un método llamado `mostrarInformacion` que imprima los valores de los atributos.
3. En el método `main` de otra clase llamada `PruebaPersona`, crea un objeto de la clase `Persona`, asigna valores a sus atributos e invoca el método `mostrarInformacion`.

#### Código sugerido:
```java
public class Persona {
    String nombre;
    int edad;

    public void mostrarInformacion() {
        System.out.println("Nombre: " + nombre);
        System.out.println("Edad: " + edad);
    }
}

public class PruebaPersona {
    public static void main(String[] args) {
        Persona persona = new Persona();
        persona.nombre = "Frank";
        persona.edad = 28;
        persona.mostrarInformacion();
    }
}
```

**Resultado Esperado:** Los valores asignados a los atributos de la clase `Persona` aparecen en la consola.

---

### Actividad 3: Uso de Tipos de Datos
**Objetivo:** Practicar con los diferentes tipos de datos en Java.

**Instrucciones:**
1. Crea una clase llamada `TiposDatos`.
2. Dentro del método `main`, declara y asigna valores a las siguientes variables:
   - Un número entero (`int`)
   - Un número decimal (`double`)
   - Un carácter (`char`)
   - Un valor lógico (`boolean`)
   - Una cadena de texto (`String`)
3. Imprime cada variable con un mensaje explicativo.

#### Código sugerido:
```java
public class TiposDatos {
    public static void main(String[] args) {
        int numeroEntero = 25;
        double numeroDecimal = 3.14;
        char caracter = 'A';
        boolean valorLogico = true;
        String texto = "Java es genial";

        System.out.println("Número Entero: " + numeroEntero);
        System.out.println("Número Decimal: " + numeroDecimal);
        System.out.println("Carácter: " + caracter);
        System.out.println("Valor Lógico: " + valorLogico);
        System.out.println("Texto: " + texto);
    }
}
```

**Resultado Esperado:** La consola muestra los valores de cada tipo de dato con un mensaje explicativo.

---

### Actividad 4: Estructuras de Programación

#### Parte 1: Declaración y Uso de Variables
**Objetivo:** Practicar la declaración y asignación de variables.

**Instrucciones:**
1. Declara y asigna valores a las variables de tipo entero, decimal, lógico y texto.
2. Imprime los valores en consola con descripciones.

#### Parte 2: Operadores
**Objetivo:** Comprender el uso de operadores aritméticos, relacionales y lógicos.

**Instrucciones:**
1. Realiza operaciones aritméticas como suma, resta y multiplicación.
2. Compara dos valores enteros con operadores relacionales (`>`, `<`, `==`, `!=`).
3. Utiliza operadores lógicos como `&&`, `||` y `!` para evaluar condiciones.

#### Código sugerido:
```java
public class Operadores {
    public static void main(String[] args) {
        int a = 10;
        int b = 20;

        System.out.println("Suma: " + (a + b));
        System.out.println("Mayor que: " + (a > b));
        System.out.println("Ambos son positivos: " + (a > 0 && b > 0));
    }
}
```

#### Parte 3: Estructuras de Control Condicional
**Objetivo:** Usar estructuras de control como `if`, `else if` y `else`.

**Instrucciones:**
1. Crea un programa que evalúe si un número ingresado por el usuario es positivo, negativo o cero.
2. Usa un bloque `if-else` para imprimir el resultado.

#### Parte 4: Estructuras de Control Repetitivas
**Objetivo:** Implementar bucles como `for`, `while` y `do-while`.

**Instrucciones:**
1. Usa un bucle `for` para imprimir los números del 1 al 10.
2. Usa un bucle `while` para sumar números hasta que alcancen un valor límite.
3. Usa un bucle `do-while` para mostrar un menú interactivo que permita realizar diferentes operaciones.

---

### Actividad 5: Creación de un Menú Interactivo con `switch`
**Objetivo:** Usar la estructura de control `switch` para crear un menú interactivo.

**Instrucciones:**
1. Crea una clase llamada `MenuInteractivo`.
2. Implementa un menú con las siguientes opciones:
   - Sumar dos números.
   - Calcular el factorial de un número.
   - Salir.
3. Usa un bucle `do-while` para que el menú siga activo hasta que el usuario elija salir.

#### Código sugerido:
```java
import java.util.Scanner;

public class MenuInteractivo {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int opcion;

        do {
            System.out.println("Menú Principal:");
            System.out.println("1. Sumar dos números");
            System.out.println("2. Calcular factorial");
            System.out.println("3. Salir");
            System.out.print("Elige una opción: ");
            opcion = scanner.nextInt();

            switch (opcion) {
                case 1:
                    System.out.print("Ingresa el primer número: ");
                    int num1 = scanner.nextInt();
                    System.out.print("Ingresa el segundo número: ");
                    int num2 = scanner.nextInt();
                    System.out.println("Resultado: " + (num1 + num2));
                    break;
                case 2:
                    System.out.print("Ingresa un número: ");
                    int num = scanner.nextInt();
                    int factorial = 1;
                    for (int i = 1; i <= num; i++) {
                        factorial *= i;
                    }
                    System.out.println("Factorial: " + factorial);
                    break;
                case 3:
                    System.out.println("Saliendo del programa...");
                    break;
                default:
                    System.out.println("Opción no válida. Intenta de nuevo.");
            }
        } while (opcion != 3);

        scanner.close();
    }
}
```

**Resultado Esperado:** Un menú interactivo que permita realizar las operaciones seleccionadas hasta que el usuario elija salir.

---

## Evaluación
- La práctica será evaluada con base en los siguientes criterios:
  - Correcta ejecución de los programas.
  - Uso adecuado de estructuras de control.
  - Implementación de menús y manejo adecuado de entradas del usuario.
  - Creatividad y claridad en el código.

