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

## Servicios relacionados

- [MentorEdu API](https://github.com/mentoredu-app/mentoredu-api) — API principal
