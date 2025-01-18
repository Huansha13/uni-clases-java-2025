# Casos Prácticos para la Sesión 1 de Java 17

### Caso 1: 
Declara dos variables numéricas (con el valor que desees), muestra por consola la `suma`, `resta`, `multiplicación`, `división` y `módulo` (resto de la división).

```java
public class OperacionesApp {

	public static void main(String[] args) {

		//Declaramos las variables
		int num1=10;
		int num2=5;

		/*Realizamos las operaciones.
		 * Tambien lo podemos guardar el resultado en variables. */

		System.out.println("El resultado de la suma es "+(num1+num2));

		System.out.println("El resultado de la resta es "+(num1-num2));

		System.out.println("El resultado de la multiplicación es "+(num1*num2));

		System.out.println("El resultado de la división es "+(num1/num2));
	}
}
```

## Caso 2: 
Declara un String que contenga tu nombre, después muestra un mensaje de bienvenida por consola. Por ejemplo: si introduzco `Julio`, me aparezca `Bienvenido Fernando`.

```java
public class SaludoApp {

	public static void main(String[] args) {

		String nombre="Fernando";

		System.out.println("Bienvenido "+nombre);
	}
}
```

## Caso 3:
Haz una aplicación que calcule el área de un círculo(pi*R2). El radio se pedirá por teclado (recuerda pasar de String a double con Double.parseDouble). Usa la constante PI y el método pow de Math.

```java
import java.util.Scanner;
public class AreaCirculoApp {
 
    public static void main(String[] args) {
 
        Scanner sc = new Scanner(System.in);
        System.out.println("Introduce un radio");
        sc.useLocale(Locale.US);
        double radio=sc.nextDouble();
 
        //Formula area circulo, usamos algunos de los metodos de Math
        double area=Math.PI*Math.pow(radio, 2);
 
        System.out.println("El area del circulo es "+area);
    }
}
```