# Monorepo VueJS + NestJS

Este es la versión inicial de un proyecto para tomar como base inicial de un proyecto del tipo monorepo con las siguientes características :

 - Presentación Vue 3 
 - Backend ( Api REST ) NestJS 
 - Conectado a base de datos MongoDB

El backend esta preparado para convertir a microservicios según la documentación de NestJS. Seguramente suba a futuro una versión de este tipo con RabbitMQ como capa de transporte.

## Estructura del proyecto

Para unificar el desarrollo de ambas capas se usó TurboRepo, un modulo que permite configurar fácilmente múltiples aplicaciones web para que funcionen como una sola permitiendo crear pipelines y distintos entornos de desarrollo.

Para la descarga de paquetes adicionales se configuraron los workspaces de proyectos, de esta manera el node_modules esta centralizado. 


**Ejemplo de descarga de paquete tailwind en la capa de presentación**

Sobre el root del proyecto ejecutamos

```
npm install -D tailwindcss --workspace fe
```

**Ejemplo de descarga de paquete microservicios en la capa de backend**

Sobre el root del proyecto ejecutamos

```
npm i @nestjs/microservices --workspace be
```

## Puesta en marcha

Clonar o descargar el proyecto y en el root del proyecto correr el comando

```
npm install
```

Para ejecutar 

```
npm run dev
```

# Futuros agregados de base

- Docker
- Logs

## Vue 3

- Pinia
- Tailwind
- Preline
- Cache VueQuery

## NestJS

- Autenticación
- Authorización
- Mongo
- Postgres / MySQL
- TypeOrm