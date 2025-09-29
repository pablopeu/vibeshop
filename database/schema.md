# 🗄️ Esquema de Base de Datos en Supabase  

## Tablas

### `productos`  
| Campo              | Tipo        | Notas                        |
|--------------------|------------|------------------------------|
| id (PK)           | uuid        | Autogenerado                 |
| nombre            | text        | Nombre del producto          |
| descripcion_corta | text        | Breve descripción            |
| descripcion_larga | text        | Detalle completo             |
| precio            | numeric     |                              |
| imagenes          | text[]      | URLs de imágenes             |
| categoria         | text        |                              |
| stock             | int         |                              |
| orden             | int         | Para ordenar en catálogo     |

### `ventas`  
| Campo    | Tipo    | Notas                               |
|----------|---------|-------------------------------------|
| id (PK) | uuid    | Autogenerado                        |
| cliente | text    | Nombre/email del cliente            |
| fecha   | timestamptz | Fecha de la venta              |
| estado  | text    | pendiente / pagado / enviado        |
| nota    | text    | Nota opcional                       |

### `configuracion`  
| Campo    | Tipo   | Notas                          |
|----------|--------|--------------------------------|
| id (PK) | uuid   | Autogenerado                   |
| clave   | text   | Ej: `hero_images`              |
| valor   | jsonb  | Configuración serializada      
