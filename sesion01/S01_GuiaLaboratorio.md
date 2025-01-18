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
        System.out.println("Operadores Aritméticos:");
        int a = 3;
        int b = a * 4;
        int c = b / 2;
        int d = c - a;
        int e = -d;
        System.out.println("a = " + a);
        System.out.println("b = " + b);
        System.out.println("c = " + c);
        System.out.println("d = " + d);
        System.out.println("e = " + e);
        System.out.println("\nOperador Módulo (residuo):");
        System.out.println("x mod 10 = " + a % 2);
        System.out.println("\nOperador Compuesto:");
        a += 2;
        b -= 4;
        c *= a;
        System.out.println("a = " + a);
        System.out.println("b = " + b);
        System.out.println("c = " + c);
        System.out.println("\nOperador Incremento:");
        ++a;
        System.out.println("a = " + a);
        ++a;
        d = b++;
        System.out.println("b = " + b);
        System.out.println("c = " + a);
        System.out.println("d = " + d);
        System.out.println("\nOperador relacional:");
        boolean res = a < b;
        System.out.println("rest = " + res);
        System.out.println("\nOperador Ternario:");
        int min = a < b ? a : b;
        System.out.println("min = " + min);
        System.out.println("\nOperador de Asignación:");
        int k = 100;
        int j = 100;
        int i = 100;
        System.out.println("i = " + i);
        System.out.println("j = " + j);
        System.out.println("k = " + k);
    }
}
```
