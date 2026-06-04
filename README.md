\# Sistema de Compras y Ventas



Proyecto fullstack desarrollado como evaluación práctica. La solución incluye un backend con NestJS basado en microservicios y un frontend con React, Vite y arquitectura modular tipo microfrontend.



\## Tecnologías principales



\### Backend



\* NestJS

\* TypeScript

\* Microservicios TCP

\* API Gateway

\* JWT

\* Swagger

\* TypeORM

\* MySQL

\* SOLID

\* DDD

\* Patrón Facade



\### Frontend



\* React

\* Vite

\* TypeScript

\* Module Federation

\* Tailwind CSS

\* Axios

\* JWT con interceptor

\* Microfrontends por dominio funcional



\## Módulos del sistema



\* Productos

\* Compras

\* Ventas

\* Movimientos

\* Kardex



\## Funcionalidades implementadas



\### Backend



\* Login con JWT con duración de 30 minutos.

\* Registro, listado y actualización de productos.

\* Registro y listado de compras.

\* Registro y listado de ventas.

\* Validación de stock en ventas.

\* Registro automático de movimientos de entrada al registrar compras.

\* Registro automático de movimientos de salida al registrar ventas.

\* Consulta de Kardex general.

\* Consulta de movimientos por producto.

\* Endpoint de stock actual por producto.

\* Documentación Swagger.

\* Collection Postman.

\* Scripts SQL.



\### Frontend



\* Login con JWT.

\* Interceptor Axios para enviar token en cada request.

\* Shell principal con menú lateral.

\* Microfrontend de productos.

\* Microfrontend de compras.

\* Microfrontend de ventas.

\* Microfrontend de Kardex.

\* Registro de compras con varios productos.

\* Registro de producto desde modal si no existe.

\* Registro de ventas validando stock disponible.

\* Visualización de Kardex y movimientos por producto.



\## Ejecución del backend



Instalar dependencias:



```bash

cd backend

npm install

```



Configurar variables de entorno:



```bash

cp .env.example .env

```



Ejecutar script SQL ubicado en:



```txt

backend/database/scripts.sql

```



Levantar servicios:



```bash

npm run start:dev productos-ms

npm run start:dev movimientos-ms

npm run start:dev compras-ms

npm run start:dev ventas-ms

npm run start:dev api-gateway

```



Swagger:



```txt

http://localhost:3000/api-docs

```



\## Ejecución del frontend



Instalar dependencias:



```bash

cd frontend

npm install

```



Levantar microfrontends:



```bash

npm run dev --workspace shell

npm run dev --workspace mfe-productos

npm run dev --workspace mfe-compras

npm run dev --workspace mfe-ventas

npm run dev --workspace mfe-kardex

```



O ejecutar cada aplicación desde su carpeta correspondiente.



Shell principal:



```txt

http://localhost:4200

```



\## Collection Postman



La colección se encuentra en:



```txt

backend/postman/Sistema\_Compras\_Ventas.postman\_collection.json

```



\## Scripts de base de datos



Los scripts se encuentran en:



```txt

backend/database/scripts.sql

```



\## Evidencias



Se incluye un video corto explicando:



\* Arquitectura del proyecto.

\* Backend con microservicios.

\* Seguridad con JWT.

\* Swagger y Postman.

\* Frontend con React, Vite y microfrontends.

\* Flujo de compras, ventas y Kardex.

\* Revisión rápida de código.



