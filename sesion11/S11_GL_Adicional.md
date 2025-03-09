# **Ejercicios Adicionales: Implementación de Interfaces en Java**

## **Ejercicio 1: Vehículos y Modo de Conducción**
**Objetivo:** Aplicar interfaces para definir el comportamiento de distintos vehículos.

### **Instrucciones:**
1. Crea una interfaz `ModoConduccion` con el método `conducir()`.
2. Implementa dos clases `Automovil` y `Motocicleta` que implementen `ModoConduccion`.
3. En `Automovil`, `conducir()` debe imprimir "El automóvil está en modo de conducción normal".
4. En `Motocicleta`, `conducir()` debe imprimir "La motocicleta está en modo deportivo".
5. Implementa una clase de prueba que cree instancias de `Automovil` y `Motocicleta` y llame a `conducir()`.

---

## **Ejercicio 2: Instrumentos Musicales y Sonido**
**Objetivo:** Aplicar interfaces para definir el comportamiento de diferentes instrumentos musicales.

### **Instrucciones:**
1. Crea una interfaz `InstrumentoMusical` con el método `tocar()`.
2. Implementa dos clases `Guitarra` y `Piano` que implementen `InstrumentoMusical`.
3. En `Guitarra`, `tocar()` debe imprimir "La guitarra está tocando un acorde".
4. En `Piano`, `tocar()` debe imprimir "El piano está tocando una melodía".
5. Implementa una clase de prueba que cree instancias de `Guitarra` y `Piano` y llame a `tocar()`.

---

## **Ejercicio 3: Dispositivos de Almacenamiento**
**Objetivo:** Aplicar interfaces para representar dispositivos de almacenamiento.

### **Instrucciones:**
1. Crea una interfaz `Almacenamiento` con los métodos `leerDatos()` y `escribirDatos(String dato)`.
2. Implementa dos clases `USB` y `DiscoDuro` que implementen `Almacenamiento`.
3. En `USB`, `leerDatos()` debe imprimir "Leyendo datos desde la memoria USB" y `escribirDatos()` debe imprimir "Guardando datos en la memoria USB".
4. En `DiscoDuro`, `leerDatos()` debe imprimir "Leyendo datos desde el disco duro" y `escribirDatos()` debe imprimir "Guardando datos en el disco duro".
5. Implementa una clase de prueba que cree instancias de `USB` y `DiscoDuro` y llame a sus métodos.

---

## **Ejercicio 4: Juegos y Consolas**
**Objetivo:** Implementar interfaces para representar el comportamiento de videojuegos en diferentes consolas.

### **Instrucciones:**
1. Crea una interfaz `Juego` con el método `iniciarJuego()`.
2. Implementa dos clases `PlayStation` y `Xbox` que implementen `Juego`.
3. En `PlayStation`, `iniciarJuego()` debe imprimir "Iniciando juego en PlayStation".
4. En `Xbox`, `iniciarJuego()` debe imprimir "Iniciando juego en Xbox".
5. Implementa una clase de prueba que cree instancias de `PlayStation` y `Xbox` y llame a `iniciarJuego()`.

---

## **Ejercicio 5: Sensores Inteligentes**
**Objetivo:** Aplicar interfaces para modelar sensores con diferentes tipos de mediciones.

### **Instrucciones:**
1. Crea una interfaz `SensorInteligente` con el método `medir()`.
2. Implementa dos clases `SensorLuz` y `SensorMovimiento` que implementen `SensorInteligente`.
3. En `SensorLuz`, `medir()` debe imprimir "Midiendo nivel de luz...".
4. En `SensorMovimiento`, `medir()` debe imprimir "Detectando movimiento...".
5. Implementa una clase de prueba que cree instancias de `SensorLuz` y `SensorMovimiento` y llame a `medir()`.
