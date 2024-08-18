# Proyecto de Recetas de Cocina

Este proyecto proporciona una aplicación que obtiene recetas de cocina detalladas y visuales. Utiliza la API de Edamam para obtener recetas, la API de Unsplash para obtener imágenes de los ingredientes y Google Generative AI para generar nombres de recetas.

## Requisitos

- Python 3.7 o superior
- Una cuenta en Google Cloud con acceso a la API de Google Generative AI
- Credenciales de servicio de Google Cloud (archivo JSON) para poder utilizar GEMINI
- Una cuenta en Unsplash con una clave de acceso a la API
- Una cuenta en Edamam con una clave de acceso a la API

## Credenciales
- Para esta preentrega deje mis credenciales de google (en el archivo googleData.json), unsplash y edamam. Así pueden probarlo de una forma mas rápida

## Instalación de Dependencias

Para ejecutar este proyecto, necesitas instalar las siguientes dependencias. Puedes hacerlo utilizando `pip`:

## Actualizaciones:
- Modifique el prompt para que puede procesar consultas en ingles y en español


```bash
pip install google-generativeai Pillow matplotlib requests
