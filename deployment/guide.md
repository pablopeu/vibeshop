# 🚀 Guía de Despliegue

## 1. Supabase
1. Crear un nuevo proyecto en [Supabase](https://supabase.com).
2. Configurar las tablas según `/database/schema.md`.
3. Guardar las credenciales (`URL` y `anon key`).

## 2. Frontend (Vercel)
1. Clonar el repo en GitHub.
2. Conectar a [Vercel](https://vercel.com).
3. Configurar variables de entorno:
   - `NEXT_PUBLIC_SUPABASE_URL`
   - `NEXT_PUBLIC_SUPABASE_ANON_KEY`
4. Deployar.

## 3. Backoffice
- Incluido en el mismo proyecto Next.js.
- Rutas protegidas con Supabase Auth.

## 4. Notas
- Se puede usar **Netlify** en lugar de Vercel.
- Monitoreo recomendado con Supabase Logs + Vercel Analytics.
