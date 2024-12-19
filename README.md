# API de Gestión de Países

## Descripción
Este proyecto es una API para gestionar y añadir información sobre países de todo el mundo. Permite realizar operaciones CRUD (Crear, Leer, Actualizar y Eliminar) en una base de datos de países. Además, se conecta con la API pública [RestCountries](https://restcountries.com/v3.1/all) para obtener datos iniciales sobre países.

## Tecnologías Utilizadas
- **Node.js**: Entorno de ejecución para JavaScript.
- **Express**: Framework para construir aplicaciones web y APIs.
- **MongoDB**: Base de datos NoSQL para almacenar la información de los países.
- **EJS**: Motor de plantillas para renderizar vistas dinámicas en la aplicación web.

## Dependencias

### Producción
- `axios`: Librería para realizar solicitudes HTTP.
- `express`: Framework minimalista para Node.js.
- `mongoose`: ODM para modelar datos en MongoDB.
- `dotenv`: Permite cargar variables de entorno desde un archivo `.env`.
- `express-ejs-layouts`: Middleware para gestionar diseños con EJS.
- `method-override`: Permite usar métodos HTTP como PUT o DELETE.
- `ejs`: Motor de plantillas.
- `express-validator`: Middleware para validar datos de solicitudes.
- `connect-flash`: Middleware para mostrar mensajes flash (por ejemplo, de error o confirmación).
- `express-session`: Middleware para gestionar sesiones en la aplicación.

### Desarrollo
- `nodemon`: Herramienta para reiniciar automáticamente la aplicación al detectar cambios en el código.

## Instalación

1. Clona este repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd <NOMBRE_DEL_REPOSITORIO>
   ```

2. Instala las dependencias:
   ```bash
   npm install
   ```

3. Configura el archivo `.env` con tus variables de entorno:
   ```env
   PORT=3000
   MONGODB_URI=<TU_URI_DE_MONGODB>
   ```

4. Inicia la aplicación en modo desarrollo:
   ```bash
   npm run dev
   ```

## Uso

### Endpoints principales
- **GET /countries**: Obtiene la lista de todos los países almacenados.
- **POST /countries**: Añade un nuevo país a la base de datos.
- **PUT /countries/:id**: Actualiza la información de un país existente.
- **DELETE /countries/:id**: Elimina un país de la base de datos.

### Conexión con la API RestCountries
La aplicación utiliza Axios para realizar solicitudes a la API de [RestCountries](https://restcountries.com/v3.1/all) y obtener datos iniciales sobre los países. Estos datos se procesan y almacenan en la base de datos MongoDB.

## Scripts

- `npm start`: Inicia la aplicación en modo producción.
- `npm run dev`: Inicia la aplicación con `nodemon` para desarrollo.

Creado por María Sofía Martín para la Diplomatura Universitaria en Full Stack con JavasCript, Nodo Tecnológico

