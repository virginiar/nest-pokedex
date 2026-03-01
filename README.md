<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

# Descripción

API REST para la gestión de Pokemons con [Nest](https://github.com/nestjs/nest).

Como base de datos se utiliza [MongoDB](https://www.mongodb.com/) en un contenedor [Docker](https://www.docker.com/).

# Ejecutar en desarrollo

1. Instalar NestJS CLI

```bash
npm i -g @nestjs/cli
```

2. Clonar el repositorio

3. Instalar las dependencias

```bash
$ npm install
```

4. Levantar la base de datos

```bash
$ docker compose up -d
```

# Compilar y ejecutar el proyecto

```bash
# desarrollo
$ npm run start

# modo observación
$ npm run start:dev

# modo producción
$ npm run build
$ npm run start:prod
```

# Aspectos analizados

En este proyecto se genera una API REST con Nest y se analizan los siguientes puntos:
- Validaciones
- CRUD contra una base de datos
- Docker y Docker compose
- Crear un volumen para conectar un contenedor con el sistema de archivos
- Esquemas y modelos
- DTOs y sus extensiones
- Uso de modelos en diferentes módulos
- SEED para rellenar la base de datos
- Paginación de resultados
- DTOs para query parameters
- Transformaciones de DTOs
- Dockerización
- Mongo Atlas
- Variables de entorno
- Esquemas de validación
- Dockerfile
- Despliegue
