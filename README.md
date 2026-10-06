# Envío de Noticias Positivas por Usuario

Solución que toma como entrada un `user_id` y envía a su correo electrónico una noticia positiva reciente sobre su categoría favorita, incluyendo un saludo personalizado, el título y el enlace a la noticia.

---

## Decisiones de diseño y optimización

* **Optimización de llamadas a la API:** Para no hacer peticiones redundantes ni saturar la cuota gratuita de Currents API, se filtran las categorías únicas de los usuarios con promociones activas.
* **Filtro de positividad:** Se excluyen noticias que contengan palabras asociadas a tragedias, violencia o crisis en su título, garantizando un contenido adecuado.
* **Validación de usuario:** La solución verifica que el usuario exista y tenga activada la opción de recibir promociones antes de procesar el envío.

---

## Requisitos previos

Instalar las librerías necesarias ejecutando en tu terminal:

```bash
pip install -r requirements.txt