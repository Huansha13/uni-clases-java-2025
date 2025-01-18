
# IDE para Desarrollo con Java 17

## IntelliJ IDEA (Community Edition)

IntelliJ IDEA es un potente entorno de desarrollo integrado (IDE) para Java, que ofrece una versión gratuita (Community Edition) adecuada para la mayoría de los desarrolladores. Es compatible con Java 17 y proporciona características avanzadas como autocompletado, depuración, integración de control de versiones, y más.

## Paso a Paso: Instalación y Configuración

### Paso 1: Descarga de JetBrains Toolbox

1. Visita la página oficial de JetBrains: [Descargar JetBrains Toolbox](https://www.jetbrains.com/toolbox-app/)
2. Descarga e instala `JetBrains Toolbox` para tu sistema operativo (Windows, macOS, Linux).

![Toolbox](..\img\img_02_Toolbox.png)

### Paso 2: Instalación de IntelliJ IDEA usando Toolbox

1. Abre `JetBrains Toolbox`.
2. Inicia sesión con tu cuenta de JetBrains o crea una nueva si no tienes una.
3. Busca `IntelliJ IDEA Community Edition` en la lista de aplicaciones disponibles.
4. Haz clic en `Install` para comenzar la instalación.
5. Una vez instalado, puedes abrir IntelliJ IDEA directamente desde Toolbox.

![Toolbox_2](..\img\img_03_Toolbox.png)

![Toolbox_2](..\img\img_04_Intellij.png)

### Paso 3: Configuración para Java 17

1. Abre IntelliJ IDEA.
2. <b>Crea un nuevo proyecto o abre uno existente.</b>
   * Ve a `File > New > Project`.
   * Selecciona `Java` y el SDK configurado (Java 17).
   * Configura el nombre del proyecto y la ubicación.
   * Haz clic en `Finish` para crear el proyecto.
3. Ve a `File > Project Structure` (o presiona `Ctrl+Alt+Shift+S`).
4. En la sección `SDKs`, haz clic en `+` y selecciona `Add JDK`.
5. Navega hasta la ruta donde tienes instalado Amazon Corretto 17 u otro JDK 17 y selecciónalo.
6. Aplica los cambios y asegúrate de que el SDK seleccionado para tu proyecto sea Java 17.

![Toolbox](..\img\img_05_Intellij_new_proyect.png)

### Paso 5: Escribir y Ejecutar un Programa Java

1. Crea un nuevo archivo Java en `src`:
   ```java
   public class Main {
       public static void main(String[] args) {
           System.out.println("¡Hola, Java 17!");
       }
   }
   ```
2. Haz clic derecho en el archivo y selecciona `Run 'Main.main()'` para ejecutar el programa.

IntelliJ IDEA facilitará el desarrollo de tus aplicaciones en Java 17 con herramientas avanzadas y una experiencia de usuario optimizada.

![Toolbox](..\img\img_06_intellij.png)

## Otros IDEs

### 1. Eclipse IDE

Eclipse es un IDE popular y gratuito para desarrollo en Java, ampliamente utilizado en la industria.

#### Paso a Paso: Instalación de Eclipse

1. Visita la página oficial de Eclipse: [Descargar Eclipse](https://www.eclipse.org/downloads/)
2. Descarga el instalador para tu sistema operativo.
3. Ejecuta el instalador y selecciona `Eclipse IDE for Java Developers`.
4. Sigue las instrucciones para completar la instalación.
5. Abre Eclipse y configura un nuevo proyecto con Java 17 siguiendo estos pasos:
   - Ve a `Window > Preferences > Java > Installed JREs`.
   - Haz clic en `Add` y selecciona `Standard VM`.
   - Navega hasta la ubicación de tu JDK 17 e introdúcelo.
   - Crea un nuevo proyecto Java y selecciona Java 17 como la JRE en uso.

### 2. Visual Studio Code (VS Code)

Visual Studio Code es un editor de código ligero y extensible que admite desarrollo en Java mediante extensiones.

#### Paso a Paso: Instalación de VS Code

1. Visita la página oficial de Visual Studio Code: [Descargar VS Code](https://code.visualstudio.com/)
2. Descarga e instala VS Code para tu sistema operativo.
3. Abre VS Code y ve a la sección de `Extensions` (o presiona `Ctrl+Shift+X`).
4. Busca e instala la extensión `Java Extension Pack`.
5. Configura tu JDK 17 en VS Code:
   - Ve a `File > Preferences > Settings`.
   - Busca `Java: Home` y establece la ruta a tu JDK 17.
6. Crea un nuevo archivo `.java` y escribe tu código. Puedes ejecutar tu programa usando la extensión.

### 3. NetBeans IDE

NetBeans es otro IDE gratuito y de código abierto para desarrollo en Java.

#### Paso a Paso: Instalación de NetBeans

1. Visita la página oficial de NetBeans: [Descargar NetBeans](https://netbeans.apache.org/download/index.html)
2. Descarga el instalador para tu sistema operativo.
3. Ejecuta el instalador y sigue las instrucciones para completar la instalación.
4. Abre NetBeans y configura un nuevo proyecto Java con los siguientes pasos:
   - Ve a `Tools > Java Platforms`.
   - Haz clic en `Add Platform` y selecciona la ubicación de tu JDK 17.
   - Crea un nuevo proyecto Java y selecciona Java 17 como la plataforma predeterminada.

Estos IDEs ofrecen distintas características que pueden ajustarse a tus necesidades de desarrollo en Java 17. 
