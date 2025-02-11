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

## Actividad 5: Calculadora de Edad
### Enunciado:
Escribe un programa en Java que solicite al usuario su año de nacimiento y calcule su edad actual.

### Solución:
```java
import java.util.Scanner;

public class CalculadoraEdad {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Ingrese su año de nacimiento: ");
        int anioNacimiento = scanner.nextInt();
        int anioActual = 2025;
        int edad = anioActual - anioNacimiento;
        System.out.println("Su edad actual es: " + edad + " años.");
        scanner.close();
    }
}
```

## Actividad 6: Área de un Rectángulo
### Enunciado:
Escribe un programa en Java que calcule el área de un rectángulo. El usuario debe ingresar la base y la altura.

### Solución:
```java
import java.util.Scanner;

public class AreaRectangulo {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Ingrese la base del rectángulo: ");
        double base = scanner.nextDouble();
        System.out.print("Ingrese la altura del rectángulo: ");
        double altura = scanner.nextDouble();
        double area = base * altura;
        System.out.println("El área del rectángulo es: " + area);
        scanner.close();
    }
}
```

## Actividad 7: Conversor de Temperatura
### Enunciado:
Crea un programa en Java que convierta una temperatura ingresada en grados Celsius a Fahrenheit.

### Solución:
```java
import java.util.Scanner;

public class ConversorTemperatura {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Ingrese la temperatura en Celsius: ");
        double celsius = scanner.nextDouble();
        double fahrenheit = (celsius * 9/5) + 32;
        System.out.println("La temperatura en Fahrenheit es: " + fahrenheit);
        scanner.close();
    }
}
```

## Actividad 8: Salario Mensual
### Enunciado:
Escribe un programa en Java que calcule el salario mensual de un empleado, dado el número de horas trabajadas y el pago por hora.

### Solución:
```java
import java.util.Scanner;

public class SalarioEmpleado {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Ingrese el número de horas trabajadas: ");
        int horas = scanner.nextInt();
        System.out.print("Ingrese el pago por hora: ");
        double pagoPorHora = scanner.nextDouble();
        double salario = horas * pagoPorHora;
        System.out.println("El salario mensual es: " + salario);
        scanner.close();
    }
}
```

## Actividad 9: Verificación de Número Par o Impar
### Enunciado:
Escribe un programa en Java que determine si un número ingresado por el usuario es par o impar.

### Solución:
```java
import java.util.Scanner;

public class ParImpar {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Ingrese un número: ");
        int numero = scanner.nextInt();
        if (numero % 2 == 0) {
            System.out.println("El número " + numero + " es par.");
        } else {
            System.out.println("El número " + numero + " es impar.");
        }
        scanner.close();
    }
}
```

# Ejercicios

### Ejercicio 1: Cálculo del Perímetro de un Círculo
Crea un programa que solicite el radio de un círculo y calcule su perímetro.

### Ejercicio 2: Conversión de Minutos a Horas
Escribe un programa que tome un número de minutos ingresado por el usuario y lo convierta a horas y minutos.

### Ejercicio 3: Comparación de Números
Solicita al usuario dos números y muestra cuál es el mayor o si son iguales.

### Ejercicio 4: Cálculo de Descuento
Crea un programa que solicite el precio de un producto y aplique un 10% de descuento.

### Ejercicio 5: Promedio de Notas
Escribe un programa que permita ingresar tres notas y calcule el promedio final.
