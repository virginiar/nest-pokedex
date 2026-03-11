<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

# Descripción

API REST para la gestión de Pokemons con [Nest](https://github.com/nestjs/nest), basado en el curso de "Nest Desarrollo Backend escalable con Node" de [DevTalles](https://cursos.devtalles.com/) en Udemy.

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

Reconstruir la base de datos con la semilla:

<http://localhost:3000/api/v2/seed>


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

## Librerías necesarias

La conexión con la base de datos MongoDB requiere de la librería [Mongoose](https://mongoosejs.com/) y del conector para NestJS:
```bash
$ npm i @nestjs/mongoose mongoose
```

Las validaciones de datos se realizan con Class-validator y class-transformer:
```bash
$ npm i class-validator class-transformer
```

Las peticiones HTTP se realizan con axios:
```bash
$ npm install axios
```
