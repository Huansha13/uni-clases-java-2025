# Ejercicios de Programación en Java

## Ejercicio 1: Calculadora de Propinas

**Enunciado:**
Escriba un programa en Java que solicite al usuario el monto de la cuenta en un restaurante y el porcentaje de propina que desea dejar. El programa debe calcular y mostrar el monto de la propina.

**Código de referencia:**
```java
import java.util.Scanner;

public class CalculadoraPropina {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Ingrese el monto de la cuenta: ");
        double cuenta = scanner.nextDouble();
        
        System.out.print("Ingrese el porcentaje de propina (ej. 15 para 15%): ");
        double porcentajePropina = scanner.nextDouble();
        
        double propina = cuenta * (porcentajePropina / 100);
        System.out.println("La propina es: " + propina);
    }
}
```

---

## Ejercicio 2: Conversor de Monedas

**Enunciado:**
Cree un programa en Java que convierta una cantidad ingresada en dólares a euros. Use un tipo de cambio fijo (por ejemplo, 1 USD = 0.85 EUR). El programa debe solicitar al usuario la cantidad en dólares y mostrar el equivalente en euros.

**Código de referencia:**
```java
import java.util.Scanner;

public class ConversorMonedas {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Ingrese la cantidad en dólares: ");
        double dolares = scanner.nextDouble();
        
        double tipoCambio = 0.85; // 1 dólar = 0.85 euros
        double euros = dolares * tipoCambio;
        
        System.out.println(dolares + " dólares son " + euros + " euros.");
    }
}
```

---

## Ejercicio 3: Calculadora de IMC (Índice de Masa Corporal)

**Enunciado:**
Desarrolle un programa en Java que calcule el Índice de Masa Corporal (IMC) de una persona a partir de su peso (kg) y su altura (m). El IMC se calcula como `peso / (altura * altura)`.

**Código de referencia:**
```java
import java.util.Scanner;

public class CalculadoraIMC {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Ingrese su peso en kg: ");
        double peso = scanner.nextDouble();
        
        System.out.print("Ingrese su altura en metros: ");
        double altura = scanner.nextDouble();
        
        double imc = peso / (altura * altura);
        System.out.println("Su IMC es: " + imc);
    }
}
```

---

## Ejercicio 4: Generador de Contraseñas Aleatorias

**Enunciado:**
Implemente un programa en Java que genere una contraseña aleatoria de 8 caracteres. La contraseña debe incluir letras mayúsculas, minúsculas y números.

**Código de referencia:**
```java
import java.util.Random;

public class GeneradorContraseña {
    public static void main(String[] args) {
        String caracteres = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789";
        Random random = new Random();
        StringBuilder contraseña = new StringBuilder();
        
        for (int i = 0; i < 8; i++) {
            int indice = random.nextInt(caracteres.length());
            contraseña.append(caracteres.charAt(indice));
        }
        
        System.out.println("Su contraseña es: " + contraseña.toString());
    }
}
```

---

## Ejercicio 5: Calculadora de Gastos Mensuales

**Enunciado:**
Escriba un programa que permita calcular los gastos mensuales de una persona en diferentes categorías como alimentos, transporte y entretenimiento. El programa debe solicitar al usuario los montos y calcular el total de gastos.

**Código de referencia:**
```java
import java.util.Scanner;

public class CalculadoraGastos {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Ingrese gastos en alimentos: ");
        double alimentos = scanner.nextDouble();
        
        System.out.print("Ingrese gastos en transporte: ");
        double transporte = scanner.nextDouble();
        
        System.out.print("Ingrese gastos en entretenimiento: ");
        double entretenimiento = scanner.nextDouble();
        
        double total = alimentos + transporte + entretenimiento;
        System.out.println("El total de gastos mensuales es: " + total);
    }
}
```

---

## Ejercicio 6: Verificador de Año Bisiesto

**Enunciado:**
Cree un programa en Java que determine si un año ingresado por el usuario es bisiesto o no. Un año es bisiesto si es divisible por 4, pero no por 100, excepto cuando también es divisible por 400.

**Código de referencia:**
```java
import java.util.Scanner;

public class VerificadorBisiesto {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Ingrese un año: ");
        int año = scanner.nextInt();
        
        boolean esBisiesto = (año % 4 == 0 && año % 100 != 0) || (año % 400 == 0);
        System.out.println(año + (esBisiesto ? " es bisiesto" : " no es bisiesto"));
    }
}
