## **Ejercicio 1: Tienda de productos**
**Objetivo:** Aplicar sobrecarga para calcular el precio total de productos con diferentes parámetros.

### **Instrucciones:**
1. Crea una clase `Tienda` con un método `calcularPrecio(int cantidad, double precioUnitario)`.
2. Sobrecarga `calcularPrecio(int cantidad, double precioUnitario, double descuento)` para aplicar descuentos.
3. Sobrecarga `calcularPrecio(int cantidad, double precioUnitario, double descuento, boolean clienteFrecuente)` para aplicar un descuento adicional si es cliente frecuente.
4. Implementa una clase de prueba y ejecuta los métodos.

---

## **Ejercicio 2: Conversión de Unidades**
**Objetivo:** Aplicar sobrecarga para convertir diferentes tipos de unidades.

### **Instrucciones:**
1. Crea una clase `Conversor` con un método `convertir(double valor, String unidadOrigen, String unidadDestino)`.
2. Sobrecarga `convertir(int valor, String unidadDestino)` para convertir desde valores enteros.
3. Sobrecarga `convertir(double valor, String unidadDestino, int decimales)` para especificar precisión en la conversión.
4. Implementa una clase de prueba con conversiones de kilómetros a millas y metros a pies.

---

## **Ejercicio 3: Sistema de Transporte**
**Objetivo:** Aplicar sobreescritura en diferentes tipos de transporte.

### **Instrucciones:**
1. Crea una clase `Transporte` con un método `viajar()` que imprima "Iniciando viaje".
2. Crea subclases `Avion`, `Barco` y `Tren` que sobrescriban `viajar()` con mensajes específicos.
3. Implementa una clase de prueba donde se creen instancias de `Avion`, `Barco` y `Tren`, llamando a `viajar()`.

---

## **Ejercicio 4: Registro de Usuarios**
**Objetivo:** Aplicar sobrecarga para registrar usuarios con distintos parámetros.

### **Instrucciones:**
1. Crea una clase `RegistroUsuarios` con un método `registrar(String nombre, String correo)`.
2. Sobrecarga `registrar(String nombre, String correo, String telefono)`.
3. Sobrecarga `registrar(String nombre, String correo, String telefono, boolean verificado)`.
4. Implementa una clase de prueba y prueba distintos métodos de registro.

---

## **Ejercicio 5: Gestión de Notificaciones**
**Objetivo:** Aplicar sobreescritura en diferentes tipos de notificaciones.

### **Instrucciones:**
1. Crea una clase `Notificacion` con un método `enviar()` que imprima "Enviando notificación genérica".
2. Crea subclases `NotificacionEmail`, `NotificacionSMS` y `NotificacionPush`.
3. Sobrescribe `enviar()` en cada subclase con mensajes específicos.
4. Implementa una clase de prueba y prueba los métodos.
