# MentorEdu File Service

Microservicio encargado de la subida y descarga de archivos (PDFs e imágenes) usando Cloudinary en producción y almacenamiento local en desarrollo.

## Stack

- Java 21 + Spring Boot 4.0.6
- Cloudinary (producción) / disco local (desarrollo)
- Docker · Render.com

## Health check

https://file-service-e9i8.onrender.com/actuator/health

## Endpoints

| Método | Ruta | Descripción |
|--------|------|-------------|
| POST | `/api/files/pdf` | Subir PDF |
| POST | `/api/files/image` | Subir imagen |
| GET | `/api/files/stream` | Descargar archivo desde Cloudinary |

## Repositorios del proyecto

| Repositorio | Descripción | Deploy |
|---|---|---|
| [mentoredu-api](https://github.com/mentoredu-app/mentoredu-api) | API REST principal | [Render](https://mentoredu-api.onrender.com/actuator/health) |
| [File-service](https://github.com/mentoredu-app/File-service) | Gestión de archivos e imágenes | [Render](https://file-service-e9i8.onrender.com/actuator/health) |
| [mentoredu-frontend](https://github.com/mentoredu-app/mentoredu-frontend) | Aplicación web | [Netlify](https://mentor-edu-frontend.netlify.app) |
| [mentoredu-landing](https://github.com/mentoredu-app/mentoredu-landing) | Landing page | [GitHub Pages](https://mentoredu-app.github.io/mentoredu-landing/) |
