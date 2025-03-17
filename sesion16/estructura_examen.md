```
TiendaApp/  
├── pom.xml
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── tienda/
│   │   │           ├── dao/
│   │   │           │   └── ProductoDAO.java
│   │   │           ├── model/
│   │   │           │   ├── Producto.java
│   │   │           │   └── Pedido.java
│   │   │           ├── service/
│   │   │           │   └── PedidoService.java
│   │   │           └── TiendaApp.java
│   │   └── resources/
│   │       └── hibernate.cfg.xml
└── README.md
```
---

### Explicación rápida:

1. **pom.xml**:
   - Incluye dependencias JDBC, Hibernate y el conector MariaDB.

2. **hibernate.cfg.xml**:
   - Configuración de Hibernate: conexión a base de datos, dialecto, usuario, password.

3. **ProductoDAO.java**:
   - Métodos para CRUD de `Producto` usando JDBC.

4. **Producto.java & Pedido.java**:
   - Clases modelo mapeadas con Hibernate (`@Entity`, `@Table`, etc.).

5. **PedidoService.java**:
   - Implementa la transacción para registrar un pedido.

6. **TiendaApp.java**:
   - Contiene el `main` con un menú simple.

¿Deseas que genere este proyecto ya empaquetado como `.zip` con configuración mínima lista? 🚀
