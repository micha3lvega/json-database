# Base de Datos de Tienda Virtual
Esta base de datos fue creada para simular un sistema de gestión de una tienda virtual. Contiene información sobre productos, clientes y órdenes.

## Estructura de la Base de Datos
La base de datos está estructurada en tres secciones principales:

1. **Productos**
   Contiene información sobre los productos disponibles en la tienda.
   Cada producto tiene un ID, un nombre, un precio y una cantidad en stock.

2. **Clientes**
   Almacena la información de los clientes registrados en la tienda.
   Cada cliente tiene un ID, un nombre y un correo electrónico.

3. **Órdenes**
   Registra las órdenes realizadas por los clientes.
   Cada orden tiene un ID, el ID del cliente que realizó la orden, una fecha, un estado y una lista de ítems que incluye el ID del producto y la cantidad.

### Cómo Utilizar
Para acceder a la base de datos y utilizarla en su proyecto, puede seguir estos pasos:

### Instalar JSON Server:
Si aún no tiene JSON Server instalado, puede hacerlo utilizando npm (Node Package Manager) con el siguiente comando:


```
npm install -g json-server
```

Iniciar el Servidor JSON:
Una vez que tenga JSON Server instalado, puede iniciar el servidor proporcionándole el archivo JSON que contiene la base de datos:

```
json-server --watch db.json
```

###  Interactuar con la API:
Una vez que el servidor esté en funcionamiento, puede acceder a la API RESTful proporcionada por JSON Server. Aquí hay algunos ejemplos de endpoints disponibles:

- /products: Obtener todos los productos.
- /products/{id}: Obtener un producto específico por su ID.
- /customers: Obtener todos los clientes.
- /customers/{id}: Obtener un cliente específico por su ID.
- /orders: Obtener todas las órdenes.
- /orders/{id}: Obtener una orden específica por su ID.

**Realizar Consultas:**
Puede realizar consultas utilizando métodos HTTP como GET, POST, PUT y DELETE para interactuar con la base de datos.

¡Y eso es todo! Ahora puede empezar a utilizar la base de datos de la tienda virtual en su proyecto.
