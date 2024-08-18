# RecIApes: Recetas Inteligentes

Este proyecto proporciona una aplicación que obtiene recetas de cocina detalladas y visuales. Utiliza la API de Edamam para obtener recetas, la API de Unsplash para obtener imágenes de los ingredientes y Google Generative AI para generar nombres de recetas.

## Requisitos

- Python 3.7 o superior
- Una cuenta en Google Cloud con acceso a la API de Google Generative AI
- Credenciales de servicio de Google Cloud (archivo JSON) para utilizar GEMINI
- Una cuenta en Unsplash con una clave de acceso a la API
- Una cuenta en Edamam con una clave de acceso a la API

## Credenciales

Para que el código funcione correctamente, necesitas obtener las credenciales correspondientes para cada API utilizada:

1. **Google Generative AI:**
   - **Pasos:**
     1. Crea una cuenta en [Google Cloud](https://cloud.google.com/).
     2. Habilita la API de Google Generative AI en tu proyecto de Google Cloud.
     3. Crea una cuenta de servicio y genera un archivo JSON de credenciales.
     4. Descarga el archivo JSON y asegúrate de almacenarlo en un lugar seguro. Este archivo es necesario para autenticar las solicitudes a la API de Google.
   - **Uso en el proyecto:**
     - Coloca el archivo JSON de credenciales en la raíz del proyecto y actualiza la variable `GOOGLE_CREDENTIALS` en el código con la ruta correspondiente.

2. **Unsplash:**
   - **Pasos:**
     1. Regístrate en [Unsplash](https://unsplash.com/developers).
     2. Crea una nueva aplicación y obtén tu clave de acceso a la API.
   - **Uso en el proyecto:**
     - Actualiza la variable `UNSPLASH_ACCESS_KEY` en el código con tu clave de acceso.

3. **Edamam:**
   - **Pasos:**
     1. Regístrate en [Edamam](https://developer.edamam.com/).
     2. Crea una nueva aplicación para obtener tu clave de API y tu ID de aplicación.
   - **Uso en el proyecto:**
     - Actualiza las variables `app_id` y `app_key` en la función `obtener_receta` con tu ID de aplicación y tu clave de API.

Para facilitar la prueba de este proyecto, he incluido mis credenciales en el archivo `googleData.json`, así como las claves de acceso para Unsplash y Edamam. Puedes utilizarlas para probar rápidamente el código, pero te recomiendo que generes tus propias credenciales para un uso continuo.

## Instalación de Dependencias

Para ejecutar este proyecto, necesitas instalar las siguientes dependencias. Puedes hacerlo utilizando `pip`:

```bash
pip install google-generativeai Pillow matplotlib requests

