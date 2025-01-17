# Ejercicios - Sobrecarga de Métodos y Constructores

## Objetivo
Practicar la sobrecarga de métodos y constructores, así como su implementación en programas con aplicaciones prácticas.

---

## Ejercicio 1: Sobrecarga de Métodos para Suma
**Instrucciones:**
1. Crea una clase llamada `Calculadora`.
2. Agrega métodos llamados `sumar` que:
   - Sumen dos enteros.
   - Sumen dos números decimales.
   - Sumen tres enteros.
3. Prueba todos los métodos en el `main`.

#### Desarrollo:
```java
public class Calculadora {
    public int sumar(int a, int b) {
        return a + b;
    }

    public double sumar(double a, double b) {
        return a + b;
    }

    public int sumar(int a, int b, int c) {
        return a + b + c;
    }
}

public class PruebaCalculadora {
    public static void main(String[] args) {
        Calculadora calc = new Calculadora();

        System.out.println("Suma de dos enteros: " + calc.sumar(5, 10));
        System.out.println("Suma de dos decimales: " + calc.sumar(3.5, 2.1));
        System.out.println("Suma de tres enteros: " + calc.sumar(1, 2, 3));
    }
}
```

---

## Ejercicio 2: Constructores con y sin Parámetros
**Instrucciones:**
1. Crea una clase `Persona` con los atributos `nombre` y `edad`.
2. Agrega un constructor sin parámetros que inicialice los valores con "Desconocido" y `0`.
3. Agrega un constructor con parámetros para inicializar los atributos.
4. Crea objetos usando ambos constructores y muestra sus datos.

#### Desarrollo:
```java
public class Persona {
    String nombre;
    int edad;

    public Persona() {
        this.nombre = "Desconocido";
        this.edad = 0;
    }

    public Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    public void mostrarInfo() {
        System.out.println("Nombre: " + nombre + ", Edad: " + edad);
    }
}

public class PruebaPersona {
    public static void main(String[] args) {
        Persona persona1 = new Persona();
        Persona persona2 = new Persona("Carlos", 25);

        persona1.mostrarInfo();
        persona2.mostrarInfo();
    }
}
```

---

## Ejercicio 3: Sobrecarga para Multiplicación
**Instrucciones:**
1. En una clase llamada `Operaciones`, crea métodos `multiplicar` que:
   - Multipliquen dos enteros.
   - Multipliquen dos números decimales.
   - Multipliquen tres números decimales.
2. Prueba cada método en el `main`.

#### Desarrollo:
```java
public class Operaciones {
    public int multiplicar(int a, int b) {
        return a * b;
    }

    public double multiplicar(double a, double b) {
        return a * b;
    }

    public double multiplicar(double a, double b, double c) {
        return a * b * c;
    }
}

public class PruebaOperaciones {
    public static void main(String[] args) {
        Operaciones op = new Operaciones();

        System.out.println("Multiplicación de enteros: " + op.multiplicar(4, 5));
        System.out.println("Multiplicación de decimales: " + op.multiplicar(2.5, 3.1));
        System.out.println("Multiplicación de tres decimales: " + op.multiplicar(1.2, 2.5, 3.3));
    }
}
```

---

## Ejercicio 4: Constructor con Varios Parámetros
**Instrucciones:**
1. Crea una clase llamada `Coche` con los atributos:
   - `marca` (String)
   - `modelo` (String)
   - `anio` (int)
   - `color` (String)
2. Agrega un constructor con todos los parámetros.
3. Crea un objeto y muestra sus datos.

#### Desarrollo:
```java
public class Coche {
    String marca;
    String modelo;
    int anio;
    String color;

    public Coche(String marca, String modelo, int anio, String color) {
        this.marca = marca;
        this.modelo = modelo;
        this.anio = anio;
        this.color = color;
    }

    public void mostrarDetalles() {
        System.out.println("Marca: " + marca);
        System.out.println("Modelo: " + modelo);
        System.out.println("Año: " + anio);
        System.out.println("Color: " + color);
    }
}

public class PruebaCoche {
    public static void main(String[] args) {
        Coche miCoche = new Coche("Toyota", "Corolla", 2020, "Rojo");
        miCoche.mostrarDetalles();
    }
}
```

---

## Ejercicio 5: Sobrecarga para Cálculo de Áreas
**Instrucciones:**
1. Crea una clase `Geometria` que tenga métodos `calcularArea` para:
   - Un cuadrado (recibe un lado).
   - Un rectángulo (recibe base y altura).
   - Un círculo (recibe el radio).

#### Desarrollo:
```java
public class Geometria {
    public double calcularArea(double lado) {
        return lado * lado;
    }

    public double calcularArea(double base, double altura) {
        return base * altura;
    }

    public double calcularAreaCirculo(double radio) {
        return Math.PI * Math.pow(radio, 2);
    }
}

public class PruebaGeometria {
    public static void main(String[] args) {
        Geometria geo = new Geometria();

        System.out.println("Área del cuadrado: " + geo.calcularArea(4));
        System.out.println("Área del rectángulo: " + geo.calcularArea(5, 3));
        System.out.println("Área del círculo: " + geo.calcularAreaCirculo(2.5));
    }
}
```

---

## Ejercicio 6: Constructores Sobrecargados para una Clase "Empleado"
**Instrucciones:**
1. Crea una clase `Empleado` con los atributos `nombre`, `edad` y `salario`.
2. Agrega los siguientes constructores:
   - Sin parámetros (asigna valores por defecto).
   - Con `nombre` y `edad`.
   - Con todos los atributos.
3. Crea objetos usando cada constructor y muestra sus datos.

#### Desarrollo:
```java
public class Empleado {
    String nombre;
    int edad;
    double salario;

    public Empleado() {
        this.nombre = "Desconocido";
        this.edad = 0;
        this.salario = 0.0;
    }

    public Empleado(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
        this.salario = 0.0;
    }

    public Empleado(String nombre, int edad, double salario) {
        this.nombre = nombre;
        this.edad = edad;
        this.salario = salario;
    }

    public void mostrarInfo() {
        System.out.println("Nombre: " + nombre + ", Edad: " + edad + ", Salario: " + salario);
    }
}

public class PruebaEmpleado {
    public static void main(String[] args) {
        Empleado e1 = new Empleado();
        Empleado e2 = new Empleado("Ana", 30);
        Empleado e3 = new Empleado("Luis", 45, 2500.50);

        e1.mostrarInfo();
        e2.mostrarInfo();
        e3.mostrarInfo();
    }
}
```