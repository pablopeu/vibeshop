# 📋 Documento de Requerimiento de Producto (PRD)

## 1. Visión General
El proyecto busca crear una tienda online moderna y administrable para la venta de cuchillos artesanales.  
La prioridad es que el sitio sea atractivo para los usuarios, fácil de navegar y, al mismo tiempo, brinde un backoffice sólido para el administrador.

Se usará **Supabase** como backend (autenticación y base de datos), lo que garantiza una solución escalable y con bajo mantenimiento. El frontend estará en **Next.js**, permitiendo rapidez, SEO optimizado y facilidad para despliegue en Vercel o Netlify.

## 2. Objetivos Principales
1. **Facilidad de uso para clientes**: la navegación debe ser simple e intuitiva, permitiendo comprar en pocos pasos.
2. **Escalabilidad técnica**: el sistema debe soportar el crecimiento en cantidad de productos y usuarios sin grandes cambios de infraestructura.
3. **Gestión integral desde el backoffice**: el administrador debe poder controlar catálogo, ventas y la imagen principal del sitio sin depender de desarrolladores.

## 3. Casos de Uso
### Cliente
- Un usuario ingresa al sitio desde su celular.  
- Ve un hero con imágenes destacadas de los cuchillos.  
- Explora el catálogo, abre el detalle de un producto, agrega unidades al carrito y completa la compra con un link de pago.  

### Administrador
- Inicia sesión en el backoffice con usuario y contraseña.  
- Revisa las ventas realizadas y marca cuáles ya están cobradas.  
- Cambia la imagen principal del hero para destacar una nueva colección.  
- Edita un producto agregando nuevas fotos y descripción más detallada.

## 4. Funcionalidades Clave
- **Frontend**:
  - Hero dinámico que se convierte en carrusel si se cargan múltiples imágenes.  
  - Catálogo con tarjetas que muestran productos y se expanden a detalle con descripción e imágenes adicionales.  
  - Carrito persistente entre sesiones y checkout con links de pago o pago presencial.  

- **Backoffice**:
  - Dashboard inicial con métricas resumidas.  
  - CRUD de productos con soporte para múltiples fotos.  
  - Gestión de ventas con actualización de estado y notas internas.  
  - Administración de imágenes y textos del hero y footer.

## 5. Requerimientos No Funcionales
- **Rendimiento**: la página debe cargar en menos de 2 segundos en conexiones promedio.  
- **Seguridad**: autenticación robusta con Supabase Auth, evitando accesos no autorizados.  
- **Escalabilidad**: hasta 10.000 usuarios concurrentes sin rediseño de arquitectura.  
- **Mantenibilidad**: el código debe estar modularizado y documentado para facilitar cambios futuros.
