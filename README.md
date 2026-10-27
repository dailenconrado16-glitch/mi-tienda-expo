# Mi Tienda — Parcial React Native / Expo

**Estudiante:** Daillent Conrado — 0182120008

Aplicación de inventario local-first para tiendas de barrio, construida con Expo SDK 54, TypeScript, Expo Router, SQLite, Drizzle y Supabase.

## Ejecutar
1. Instalar Node.js LTS y Expo Go compatible con SDK 54.
2. Crear un proyecto propio en Supabase. En Authentication > Providers > Email, desactivar confirmación por correo para las pruebas del parcial.
3. Ejecutar `supabase/schema.sql` en SQL Editor (una sola vez).
4. Copiar `.env.example` a `.env` y completar **URL** y **publishable key** (nunca secret/service_role).
5. Ejecutar `npm install` y `npx expo start`; abrir QR con Expo Go.
6. Registrar una cuenta, ingresar, agregar productos y tocar Sincronizar.

## Funcionalidades implementadas en código
- Registro, login, logout y persistencia en SecureStore.
- Stack.Protected, rutas para sesión y visitante.
- Migración SQLite, repositorio Drizzle, useLiveQuery y CRUD local sin conexión.
- Totales, búsqueda, indicadores pendientes y confirmación de eliminación.
- Sincronización manual: descargar faltantes, subir pendientes con upsert.
- RLS por usuario en Supabase.

## Limitaciones y comprobaciones pendientes
- Requiere proyecto Supabase y credenciales reales para ejecutar autenticación/sincronización.
- Borrado en la nube no implementado (fuera de alcance del parcial).
- Resolución de conflictos entre dos dispositivos no implementada (fuera de alcance).
- Las capturas deben tomarse en el teléfono y panel de Supabase después de probar la app. No se incluyen imágenes simuladas.
- No se ha validado una ejecución real en Expo Go desde este entorno.

## Capturas requeridas
![Login](capturas/01-login.png)
![Registro](capturas/02-registro.png)
![Principal](capturas/03-principal.png)
![Formulario](capturas/04-formulario.png)
![Sin conexión](capturas/05-sin-conexion.png)
![Sincronizado](capturas/06-sincronizado.png)
![Supabase](capturas/07-supabase.png)

## GitHub
Crear repositorio público `parcial-mi-tienda-<apellido>` y hacer al menos 4 commits descriptivos. Verificar `git status` y que `.env` no esté rastreado.
