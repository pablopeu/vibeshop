# 🗄️ Esquema de Base de Datos en Supabase  

## Tablas y Descripción

### `productos`  
Almacena todos los datos relacionados con los productos que se ofrecen en la tienda.  
Incluye campos de nombre, descripciones, precio, imágenes múltiples y un campo `orden` que permite controlar el orden de visualización en el catálogo.

### `ventas`  
Representa cada transacción realizada en el sitio.  
Guarda información del cliente, fecha de la operación, estado actual y una nota opcional para los administradores.  
La gestión de este estado es central para el backoffice, permitiendo llevar control de las ventas.

### `configuracion`  
Tabla genérica para almacenar configuraciones del sistema.  
Ejemplos: imágenes del hero/carrousel, textos de footer, opciones de FAQ y WhatsApp.  
Se usa un campo `jsonb` en `valor` para poder manejar datos flexibles.

---

## Relaciones y Consideraciones
- `ventas` puede referenciar productos, pero inicialmente se registrará como una transacción independiente para simplificar.  
- `configuracion` es clave para dar flexibilidad sin requerir cambios constantes en la base.  
- El uso de UUIDs permite escalabilidad y evita colisiones.
