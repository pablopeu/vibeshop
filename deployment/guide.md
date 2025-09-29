# 🚀 Guía de Despliegue

## 1. Supabase
1. Crear un nuevo proyecto en [Supabase](https://supabase.com).  
2. Configurar las tablas siguiendo `/database/schema.md`.  
3. Guardar las credenciales (`URL` y `anon key`). Estas serán usadas por el frontend.  

La elección de Supabase se debe a que provee autenticación, base de datos y almacenamiento en un solo servicio, reduciendo la complejidad del backend.

## 2. Frontend (Vercel)
1. Clonar el repo en GitHub.  
2. Conectar a [Vercel](https://vercel.com).  
3. Configurar variables de entorno en Vercel:  
   - `NEXT_PUBLIC_SUPABASE_URL`  
   - `NEXT_PUBLIC_SUPABASE_ANON_KEY`  
4. Deploy automático con cada push a la rama principal.

La ventaja de Vercel es la integración nativa con Next.js, que permite builds optimizados y despliegues rápidos.

## 3. Backoffice
- El backoffice estará dentro del mismo proyecto Next.js.  
- Se protegerán rutas mediante Supabase Auth.  
- El admin ingresará con credenciales definidas en Supabase.

## 4. Notas
- También puede usarse **Netlify** si se prefiere, con configuración similar.  
- Para monitoreo, se recomienda usar **Supabase Logs** y **Vercel Analytics**.  
- Se puede configurar un flujo CI/CD para que cada actualización en GitHub se despliegue automáticamente.
