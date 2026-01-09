# Fast Food API

API desarrollada con **NestJS** para la gestión de productos, ventas y reportes de un sistema de comida rápida.  
El proyecto maneja **stock**, **ventas**, **validaciones** y **reportes**, y está documentado con **Swagger**.



## Tecnologías utilizadas

- **Node.js**
- **NestJS**
- **TypeScript**
- **TypeORM**
- **PostgreSQL**
- **Swagger (OpenAPI)**
- **class-validator / class-transformer**

---

## Funcionalidades principales

  ### Productos
  - Crear productos
  - Obtener todos los productos
  - Obtener productos disponibles (stock > 0)
  - Obtener producto por ID
  - Actualizar productos
  - Eliminar productos

  ---

  ### Ventas
  - Registrar una venta
  - Cálculo automático del total
  - Validación de stock disponible
  - Descuento de stock al realizar una venta
  - Obtener ventas
  - Actualizar y eliminar ventas

  ---

  ###  Reportes
  - Total de ventas del sistema
  - Producto más vendido


##  Endpoints principales

  ### Productos
  - GET /productos
  - GET /productos/disponibles
  - GET /productos/:id
  - POST /productos
  - PUT /productos/:id
  - DELETE /productos/:id

  ### Ventas
  - GET /ventas
  - GET /ventas/:id
  - POST /ventas
  - PUT /ventas/:id
  - DELETE /ventas/:id

  ### Reportes
  - GET /reportes/ventas-totales
  - GET /reportes/producto-mas-vendido


## Validaciones

  - Validación automática de datos con `ValidationPipe`
  - Uso de DTOs (`CreateDto`, `UpdateDto`)
  - Control de errores con excepciones HTTP
  - Prevención de propiedades no permitidas

---

## Documentación con Swagger

  Una vez iniciado el proyecto, se puede acceder a la documentación en:
  http://localhost:3000/api

## Cómo ejecutar el proyecto

  1. Instalar dependencias:
    npm install

  2. Configurar la base de datos en el archivo .env

  3. Ejecutar el proyecto:
    npm run start:dev

## Autor

  Desarrollado por Diego Ruda  
