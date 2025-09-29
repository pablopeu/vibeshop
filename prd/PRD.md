# 📋 Documento de Requerimiento de Producto (PRD)

## 1. Visión General
- Crear un ecommerce minimalista, escalable y administrable para vender cuchillos artesanales.
- El sistema debe tener:
  - **Frontend**: catálogo, carrito, checkout, hero dinámico.
  - **Backoffice**: gestión de productos, ventas, hero images.
  - **Base de datos**: centralizada en Supabase.
  - **Deployment**: deploy serverless (Vercel/Netlify + Supabase).

## 2. Objetivos Principales
- Facilidad de uso en frontend (UX intuitiva).
- Escalabilidad en backend (Supabase).
- Control total para administrador vía backoffice.

## 3. Casos de Uso
1. **Cliente**:
   - Navega productos.
   - Añade al carrito.
   - Realiza compra.
2. **Administrador**:
   - Gestiona productos (CRUD).
   - Administra ventas (actualizar estado, notas).
   - Cambia imágenes del hero/carrousel.

## 4. Funcionalidades Clave
- **Frontend**:
  - Hero dinámico con imágenes administrables.
  - Catálogo con múltiples imágenes por producto.
  - Carrito y checkout básico.
- **Backoffice**:
  - Dashboard con métricas.
  - CRUD de productos.
  - Gestión de ventas y estados.
  - Configuración de hero images.

## 5. Requerimientos No Funcionales
- **Rendimiento**: carga rápida (<2s).
- **Seguridad**: autenticación segura (Supabase Auth).
- **Escalabilidad**: soportar hasta 10k usuarios sin cambios de arquitectura.
- **Mantenibilidad**: código modular y documentado.
