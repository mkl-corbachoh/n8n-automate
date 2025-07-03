# Configuración de n8n con Docker

Este repositorio contiene los archivos de configuración necesarios para ejecutar n8n usando Docker.

## Requisitos previos

- Docker
- Docker Compose

## Configuración

La configuración utiliza las siguientes variables de entorno (definidas en `.env`):
- `N8N_HOST`: El host donde se ejecutará n8n (por defecto: localhost)
- `N8N_ENCRYPTION_KEY`: Una clave de cifrado aleatoria (mínimo 32 caracteres)

## Primeros pasos

1. Asegúrate de tener Docker y Docker Compose instalados en tu sistema
2. Actualiza el archivo `.env` con tu configuración deseada
3. Ejecuta n8n usando Docker Compose:
```bash
docker-compose up -d
```

4. Accede a n8n en http://localhost:5678

## Almacenamiento

Todos los datos de n8n se guardan en un volumen de Docker llamado `n8n_data`.
