# Proyecto de Recetas de Cocina

Este proyecto proporciona una aplicación que obtiene recetas de cocina detalladas y visuales. Utiliza la API de Edamam para obtener recetas, la API de Unsplash para obtener imágenes de los ingredientes y Google Generative AI para generar nombres de recetas.

## Requisitos

- Python 3.7 o superior
- Una cuenta en Google Cloud con acceso a la API de Google Generative AI
- Credenciales de servicio de Google Cloud (archivo JSON) para poder utilizar GEMINI
- Una cuenta en Unsplash con una clave de acceso a la API
- Una cuenta en Edamam con una clave de acceso a la API

## Credenciales

Para ejecutar este proyecto, necesitarás proporcionar tus propias credenciales de Google Cloud, Unsplash y Edamam. Sigue las instrucciones a continuación para configurar estas credenciales.

### Configuración de Credenciales

1. **Credenciales de Google Cloud**:
   - Accede a tu consola de Google Cloud y crea una nueva cuenta de servicio con los permisos necesarios.
   - Descarga el archivo JSON con las credenciales de la cuenta de servicio.
   - Renombra este archivo a `googleData.json` y colócalo en la raíz del proyecto.

2. **Credenciales de Unsplash**:
   - Crea una cuenta en Unsplash y genera una clave de acceso a la API.
   - Guarda esta clave en una variable de entorno llamada `UNSPLASH_ACCESS_KEY`.

3. **Credenciales de Edamam**:
   - Crea una cuenta en Edamam y genera una clave de acceso a la API.
   - Guarda el ID de la aplicación y la clave en variables de entorno llamadas `EDAMAM_APP_ID` y `EDAMAM_APP_KEY`.

Para configurar las variables de entorno, puedes añadirlas a tu archivo de configuración o exportarlas en tu terminal de la siguiente manera:

```bash
export UNSPLASH_ACCESS_KEY='tu_unsplash_access_key'
export EDAMAM_APP_ID='tu_edamam_app_id'
export EDAMAM_APP_KEY='tu_edamam_app_key'