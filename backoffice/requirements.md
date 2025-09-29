# 🛡️ Requerimientos del Backoffice

## 1. General
El backoffice es la herramienta de gestión del administrador.  
Debe ser accesible con autenticación segura (Supabase Auth) y diseñado con **Next.js**.  

## 2. Módulos
### Dashboard
- Pantalla inicial con métricas clave: cantidad de ventas, productos activos y pendientes.  
- Permite una visión rápida del estado del negocio.

### Gestión de productos
- CRUD completo: crear, editar, eliminar y listar productos.  
- Subida de múltiples imágenes por producto.  
- Posibilidad de ordenar productos en catálogo.  

### Gestión de ventas
- Listado de todas las ventas con posibilidad de filtrarlas por estado.  
- Actualización de estado: pendiente, cobrada, enviada.  
- Campo de notas internas que ayuda a la comunicación entre administradores.  
- Capacidad de revertir una venta marcada como cobrada a pendiente.  

### Gestión de hero/carrousel
- Subida de imágenes para el hero.  
- Si hay más de una, se convierten en carrusel automático.  
- Opción de agregar descripciones y ordenarlas.

### Configuración del footer
- Todo el texto de información de la tienda en el footer será editable desde este módulo.

## 3. Requerimientos UX
- Panel minimalista, con navegación lateral clara.  
- Compatible con escritorio y tablet.  
- Botón superior para abrir el sitio público en una nueva pestaña.

## 4. Seguridad
- Acceso solo para usuarios con rol administrador en Supabase Auth.  
- Datos sensibles encriptados y gestionados vía Supabase.
