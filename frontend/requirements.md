# 🎨 Requerimientos del Frontend

## 1. General
El frontend será desarrollado con **Next.js** y **TailwindCSS**, lo que asegura velocidad, flexibilidad en el diseño y soporte SEO. La autenticación se gestionará con **Supabase Auth**.

## 2. Páginas Principales
### Home
- Presenta un **hero** visualmente atractivo.  
- Si hay más de una imagen configurada, se convierte en un **carrusel automático** que rota cada 5 segundos.  
- Incluye un grid de productos destacados para captar la atención de los usuarios.

### Catálogo
- Lista completa de productos con opción de filtros.  
- Cada tarjeta abre un detalle en overlay o modal, donde se ven imágenes adicionales y descripciones completas.  
- El overlay debe permitir seleccionar cantidad y añadir al carrito, cerrándose para volver al catálogo.

### Detalle de producto
- Muestra imágenes adicionales, precio y descripciones largas.  
- Incluye botones de acción claros (añadir al carrito, volver al catálogo).

### Carrito y Checkout
- El carrito debe ser persistente con localStorage.  
- Checkout simple que redirige a links de pago o permite seleccionar pago presencial.  

## 3. Requerimientos UX
- El diseño debe ser **responsive** y optimizado para móviles.  
- La navegación debe ser clara, con botones visibles para “añadir al carrito” y “comprar”.  
- Deben existir accesos rápidos a preguntas frecuentes (FAQ) y WhatsApp de contacto.

## 4. Integraciones
El frontend se conecta con Supabase para:  
- Obtener productos y sus configuraciones.  
- Consultar imágenes del hero/carrousel.  
- Sincronizar ventas realizadas.
