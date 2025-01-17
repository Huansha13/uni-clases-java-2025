# Métodos y Variables Estáticos

## Ejercicios

### Ejercicio 1: Creación de un Método Estático
**Objetivo**: Implementar un método estático que calcule el área de un círculo.

```java
public class Matematica {
    public static double calcularAreaCirculo(double radio) {
        return Math.PI * radio * radio;
    }
}

// Uso del método estático
System.out.println("Área del círculo: " + Matematica.calcularAreaCirculo(5));
```

### Ejercicio 2: Uso de una Variable Estática
**Objetivo**: Crear una clase `Empleado` que tenga una variable estática para contar cuántos empleados se han creado.

```java
public class Empleado {
    private String nombre;
    public static int contadorEmpleados = 0;

    public Empleado(String nombre) {
        this.nombre = nombre;
        contadorEmpleados++;
    }

    public String getNombre() {
        return nombre;
    }
}

// Creación de instancias y comprobación del contador
Empleado e1 = new Empleado("Ana");
Empleado e2 = new Empleado("Luis");
System.out.println("Número de empleados: " + Empleado.contadorEmpleados); // Imprime 2
```

### Ejercicio 3: Comparación entre Métodos Estáticos y No Estáticos
**Objetivo**: Implementar métodos estáticos y no estáticos en la misma clase y demostrar sus diferencias.

```java
public class Operaciones {
    public static int sumar(int a, int b) {
        return a + b;
    }

    public int multiplicar(int a, int b) {
        return a * b;
    }
}

// Llamada al método estático
int suma = Operaciones.sumar(5, 10);

// Creación de una instancia para llamar al método no estático
Operaciones op = new Operaciones();
int multiplicacion = op.multiplicar(5, 10);
```

### Ejercicio 4: Contador de Instancias
**Objetivo**: Crear una clase `Vehiculo` con una variable estática que cuente cuántos vehículos se han creado.

```java
public class Vehiculo {
    private String modelo;
    public static int contadorVehiculos = 0;

    public Vehiculo(String modelo) {
        this.modelo = modelo;
        contadorVehiculos++;
    }

    public String getModelo() {
        return modelo;
    }
}

// Creación de instancias y comprobación del contador
Vehiculo v1 = new Vehiculo("Toyota Corolla");
Vehiculo v2 = new Vehiculo("Honda Civic");
System.out.println("Número de vehículos: " + Vehiculo.contadorVehiculos); // Imprime 2
```

### Ejercicio 5: Uso de Métodos Estáticos para Utilidades
**Objetivo**: Crear una clase `Conversor` con métodos estáticos para convertir unidades (por ejemplo, de kilómetros a millas).

```java
public class Conversor {
    public static double kilometrosAMillas(double kilometros) {
        return kilometros * 0.621371;
    }

    public static double millasAKilometros(double millas) {
        return millas / 0.621371;
    }
}

// Uso de métodos estáticos
System.out.println("10 kilómetros son " + Conversor.kilometrosAMillas(10) + " millas.");
System.out.println("6.2 millas son " + Conversor.millasAKilometros(6.2) + " kilómetros.");
```

### Ejercicio 6: Creación de un Banco de Nombres
**Objetivo**: Crear una clase `NombreBanco` con una variable estática que almacene una lista de nombres y métodos para agregar y mostrar los nombres.

```java
import java.util.ArrayList;

public class NombreBanco {
    private static ArrayList<String> nombres = new ArrayList<>();

    public static void agregarNombre(String nombre) {
        nombres.add(nombre);
    }

    public static void mostrarNombres() {
        for (String nombre : nombres) {
            System.out.println(nombre);
        }
    }
}

// Uso de métodos estáticos
NombreBanco.agregarNombre("Carlos");
NombreBanco.agregarNombre("María");
NombreBanco.mostrarNombres();
```

### Ejercicio 7: Contador de Palabras
**Objetivo**: Implementar una clase `ContadorPalabras` con un método estático que cuente el número de palabras en una cadena.

```java
public class ContadorPalabras {
    public static int contarPalabras(String frase) {
        if (frase == null || frase.isEmpty()) {
            return 0;
        }
        String[] palabras = frase.split("\\s+");
        return palabras.length;
    }
}

// Uso del método estático
System.out.println("Número de palabras: " + ContadorPalabras.contarPalabras("Hola mundo desde Java"));
```

### Ejercicio 8: Validación de Correos Electrónicos
**Objetivo**: Crear una clase `Validador` con un método estático que valide si una dirección de correo electrónico es válida.

```java
public class Validador {
    public static boolean esCorreoValido(String correo) {
        return correo.matches("^[\\w._%+-]+@[\\w.-]+\\.[a-zA-Z]{2,6}$");
    }
}

// Uso del método estático
System.out.println("Correo válido: " + Validador.esCorreoValido("test@example.com"));
System.out.println("Correo válido: " + Validador.esCorreoValido("correo@@ejemplo.com"));
```

### Ejercicio 9: Generación de Identificadores Únicos
**Objetivo**: Implementar una clase `IdentificadorUnico` con un método estático que genere un identificador único incremental.

```java
public class IdentificadorUnico {
    private static int idActual = 0;

    public static int generarId() {
        return ++idActual;
    }
}

// Uso del método estático
System.out.println("ID generado: " + IdentificadorUnico.generarId());
System.out.println("ID generado: " + IdentificadorUnico.generarId());
```

### Ejercicio 10: Calculadora de Factorial
**Objetivo**: Crear una clase `Calculadora` con un método estático que calcule el factorial de un número.

```java
public class Calculadora {
    public static long calcularFactorial(int numero) {
        if (numero <= 1) {
            return 1;
        }
        return numero * calcularFactorial(numero - 1);
    }
}

// Uso del método estático
System.out.println("Factorial de 5: " + Calculadora.calcularFactorial(5));
System.out.println("Factorial de 0: " + Calculadora.calcularFactorial(0));
```

### Ejercicio 11: Suma de Números en un Array
**Objetivo**: Crear una clase `Utilidades` con un método estático que calcule la suma de todos los números en un array.

```java
public class Utilidades {
    public static int sumarArray(int[] numeros) {
        int suma = 0;
        for (int numero : numeros) {
            suma += numero;
        }
        return suma;
    }
}

// Uso del método estático
int[] numeros = {1, 2, 3, 4, 5};
System.out.println("Suma de números: " + Utilidades.sumarArray(numeros));
```

### Ejercicio 12: Conversión de Temperaturas
**Objetivo**: Crear una clase `ConversorTemperaturas` con métodos estáticos para convertir entre Celsius y Fahrenheit.

```java
public class ConversorTemperaturas {
    public static double celsiusAFahrenheit(double celsius) {
        return (celsius * 9/5) + 32;
    }

    public static double fahrenheitACelsius(double fahrenheit) {
        return (fahrenheit - 32) * 5/9;
    }
}

// Uso de métodos estáticos
System.out.println("25°C a Fahrenheit: " + ConversorTemperaturas.celsiusAFahrenheit(25));
System.out.println("77°F a Celsius: " + ConversorTemperaturas.fahrenheitACelsius(77));
```

### Ejercicio 13: Verificación de Números Primos
**Objetivo**: Crear una clase `MatematicaAvanzada` con un método estático que determine si un número es primo.

```java
public class MatematicaAvanzada {
    public static boolean esPrimo(int numero) {
        if (numero <= 1) {
            return false;
        }
        for (int i = 2; i <= Math.sqrt(numero); i++) {
            if (numero % i == 0) {
                return false;
            }
        }
        return true;
    }
}

// Uso del método estático
System.out.println("¿Es primo 7? " + MatematicaAvanzada.esPrimo(7));
System.out.println("¿Es primo 10? " + MatematicaAvanzada.esPrimo(10));
```

### Ejercicio 14: Cálculo de Potencias
**Objetivo**: Implementar una clase `CalculadoraPotencia` con un método estático que calcule la potencia de un número dado.

```java
public class CalculadoraPotencia {
    public static double calcularPotencia(double base, int exponente) {
        return Math.pow(base, exponente);
    }
}

// Uso del método estático
System.out.println("2^3: " + CalculadoraPotencia.calcularPotencia(2, 3));
System.out.println("5^4: " + CalculadoraPotencia.calcularPotencia(5, 4));
```

### Ejercicio 15: Cálculo de Promedio
**Objetivo**: Crear una clase `Estadisticas` con un método estático que calcule el promedio de un array de números.

```java
public class Estadisticas {
    public static double calcularPromedio(int[] numeros) {
        if (numeros.length == 0) {
            return 0;
        }
        int suma = 0;
        for (int numero : numeros) {
            suma += numero;
        }
        return (double) suma / numeros.length;
    }
}

// Uso del método estático
int[] datos = {10, 20, 30, 40, 50};
System.out.println("Promedio: " + Estadisticas.calcularPromedio(datos));
```
