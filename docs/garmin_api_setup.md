# Configuración de Garmin Connect API

Este documento explica cómo obtener credenciales para integrar **Data Deportiva** con Garmin Connect.

---

## 1. Crear cuenta de desarrollador Garmin

1. Ir a [https://developer.garmin.com/](https://developer.garmin.com/).
2. Crear una cuenta o iniciar sesión.
3. Acceder a **Garmin Connect Developer Program**.

---

## 2. Registrar una nueva aplicación

1. En el panel de desarrollador, seleccionar **Create a New Application**.
2. Completar los campos requeridos:
   - **Application Name:** Data Deportiva
   - **Application Website:** `https://datadeportiva.pro`
   - **Privacy Policy URL:** `https://datadeportiva.pro/privacy-policy`
   - **Contact Email:** `contacto@datadeportiva.pro`
   - **Redirect URI:** `http://localhost:3000/auth/garmin/callback` (para desarrollo) y la de producción.
3. Seleccionar permisos requeridos:
   - `activity`
   - `health`
   - `profile`

---

## 3. Obtener credenciales

Una vez aprobada la app, Garmin entregará:
- `Client ID`
- `Client Secret`

Agregarlos en el archivo `.env`:

```bash
GARMIN_CLIENT_ID=tu_client_id
GARMIN_CLIENT_SECRET=tu_client_secret
