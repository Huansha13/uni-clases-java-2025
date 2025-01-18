# Casos Prácticos para la Sesión 1 de Java 17

## Caso 1: Conversión de Temperatura

**Enunciado:** Escribe un programa que convierta grados Celsius a Fahrenheit.  
**Requerimiento:** El programa debe solicitar al usuario una temperatura en grados Celsius y mostrar la conversión en grados Fahrenheit.

```java
import java.util.Scanner;

public class CelsiusToFahrenheit {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce la temperatura en Celsius: ");
        double celsius = scanner.nextDouble();
        double fahrenheit = (celsius * 9/5) + 32;
        System.out.println("La temperatura en Fahrenheit es: " + fahrenheit);
    }
}
```

## Caso 2: Cálculo del Área de un Círculo

**Enunciado:** Calcula el área de un círculo dada su radio.  
**Requerimiento:** El programa debe leer el radio del usuario y calcular el área usando la fórmula πr².

```java
import java.util.Scanner;

public class AreaCirculo {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce el radio del círculo: ");
        double radio = scanner.nextDouble();
        double area = Math.PI * Math.pow(radio, 2);
        System.out.println("El área del círculo es: " + area);
    }
}
```

## Caso 4: Calculadora de Suma

**Enunciado:** Implementa una calculadora que sume dos números.  
**Requerimiento:** El programa debe leer dos números y mostrar su suma.

```java
import java.util.Scanner;

public class CalculadoraSuma {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce el primer número: ");
        int num1 = scanner.nextInt();
        System.out.print("Introduce el segundo número: ");
        int num2 = scanner.nextInt();
        int suma = num1 + num2;
        System.out.println("La suma de los números es: " + suma);
    }
}
```

## Caso 5: Verificar si un Número es Par o Impar

**Enunciado:** Determina si un número es par o impar.  
**Requerimiento:** El programa debe solicitar un número y verificar si es par o impar.

```java
import java.util.Scanner;

public class ParOImpar {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce un número: ");
        int num = scanner.nextInt();

        if (num % 2 == 0) {
            System.out.println("El número es par.");
        } else {
            System.out.println("El número es impar.");
        }
    }
}
```

## Caso 6: Calcular el Factorial de un Número

**Enunciado:** Calcula el factorial de un número entero no negativo.  
**Requerimiento:** El programa debe leer un número y calcular su factorial.

```java
import java.util.Scanner;

public class Factorial {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce un número entero no negativo: ");
        int num = scanner.nextInt();
        long factorial = 1;

        for (int i = 1; i <= num; i++) {
            factorial *= i;
        }

        System.out.println("El factorial de " + num + " es: " + factorial);
    }
}
```

## Caso 7: Calcular Promedio de Tres Números

**Enunciado:** Calcula el promedio de tres números ingresados por el usuario.  
**Requerimiento:** El programa debe solicitar tres números y calcular su promedio.

```java
import java.util.Scanner;

public class PromedioTresNumeros {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce el primer número: ");
        double num1 = scanner.nextDouble();
        System.out.print("Introduce el segundo número: ");
        double num2 = scanner.nextDouble();
        System.out.print("Introduce el tercer número: ");
        double num3 = scanner.nextDouble();
        double promedio = (num1 + num2 + num3) / 3;
        System.out.println("El promedio es: " + promedio);
    }
}
```

## Caso 8: Determinar el Año Bisiesto

**Enunciado:** Determina si un año ingresado por el usuario es bisiesto.  
**Requerimiento:** El programa debe verificar si el año es divisible por 4 pero no por 100, o si es divisible por 400.

```java
import java.util.Scanner;

public class AnoBisiesto {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce un año: ");
        int ano = scanner.nextInt();

        if ((ano % 4 == 0 && ano % 100 != 0) || (ano % 400 == 0)) {
            System.out.println("El año " + ano + " es bisiesto.");
        } else {
            System.out.println("El año " + ano + " no es bisiesto.");
        }
    }
}
```

## Caso 9: Invertir una Cadena de Texto

**Enunciado:** Escribe un programa que invierta una cadena de texto ingresada por el usuario.  
**Requerimiento:** El programa debe leer una cadena y mostrarla invertida.

```java
import java.util.Scanner;

public class InvertirCadena {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce una cadena de texto: ");
        String cadena = scanner.nextLine();
        String invertida = new StringBuilder(cadena).reverse().toString();
        System.out.println("La cadena invertida es: " + invertida);
    }
}
```

## Caso 10: Calcular Potencia de un Número

**Enunciado:** Calcula la potencia de un número base elevado a un exponente.  
**Requerimiento:** El programa debe leer una base y un exponente, y calcular la potencia.

```java
import java.util.Scanner;

public class CalcularPotencia {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce la base: ");
        double base = scanner.nextDouble();
        System.out.print("Introduce el exponente: ");
        int exponente = scanner.nextInt();
        double resultado = Math.pow(base, exponente);
        System.out.println("El resultado es: " + resultado);
    }
}
```