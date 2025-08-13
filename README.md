# Data Deportiva

**Data Deportiva** es una plataforma B2B que integra datos de entrenamiento desde **Garmin Connect** y los interpreta automáticamente mediante Inteligencia Artificial para generar reportes claros, accionables y listos para compartir con entrenadores, clubes y deportistas.

Nuestro objetivo es **ahorrar tiempo en la gestión y análisis de datos** y facilitar la toma de decisiones basada en métricas precisas.

---

## 🚀 Características principales

- **Integración automática con Garmin Connect** (OAuth 2.0).
- **Procesamiento de datos** con análisis avanzado y segmentación por métricas clave.
- **Reportes automatizados** con interpretaciones de IA listos para enviar.
- **Panel de control** para visualizar y descargar informes.
- **Diseñado para entrenadores, clubes y organizaciones deportivas** (no uso personal).

---

## 📦 Estructura del proyecto

- `/src` — Código fuente principal.
- `/docs` — Documentación técnica y guías de uso.
- `/flows` — Flujos de automatización (internamente con n8n).
- `/db` — Scripts y esquemas de base de datos (PostgreSQL).
- `/public` — Recursos públicos (imágenes, logos, etc.).

---

## 🛠 Tecnologías

- **Backend:** Node.js + Express
- **Base de datos:** PostgreSQL
- **Integración API:** Garmin Connect (OAuth 2.0)
- **Automatización interna:** n8n (no visible para clientes)
- **IA:** ChatGPT para interpretación de datos

---

## 🔐 Requisitos previos

- Node.js >= 18
- PostgreSQL >= 14
- Credenciales de Garmin Connect API (ver `/docs/garmin_api_setup.md`)
- Variables de entorno configuradas en `.env`

---

## ⚙️ Instalación y ejecución

```bash
# Clonar el repositorio
git clone https://github.com/usuario/data-deportiva.git
cd data-deportiva

# Instalar dependencias
npm install

# Configurar variables de entorno
cp .env.example .env
# Editar .env con credenciales correctas

# Ejecutar en desarrollo
npm run dev

# Compilar y ejecutar en producción
npm run build
npm start
