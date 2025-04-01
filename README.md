# Proyecto Backend (Laravel 8)

Este proyecto tiene un **backend en Laravel 8** y un **frontend en Angular**. A continuación se detallan los pasos para instalar, configurar y ejecutar ambos proyectos, así como los comandos necesarios.

## Backend - Laravel 8

### Requisitos del Sistema

- PHP 7.3 o superior
- Composer (para manejar las dependencias de PHP)
- MySQL o cualquier base de datos compatible con Laravel
- Node.js (para la compilación de assets si es necesario)
- npm o yarn (para la gestión de dependencias de frontend si es necesario)

### Instalación del Backend

1. **Clonar el Repositorio**

   Clona el repositorio del backend desde GitHub:
   ```bash
   git clone https://github.com/els1203/Ecommer.git
   cd backend-repo

2. Instalar las Dependencias de PHP

Ejecuta el siguiente comando para instalar las dependencias de PHP usando Composer:
composer install

3. Configurar el Archivo .env

Copia el archivo .env.example a .env:
cp .env.example .env

Abre el archivo .env y configura la base de datos, el correo electrónico y otros parámetros:

Base de datos:

DB_CONNECTION=mysql

DB_HOST=127.0.0.1

DB_PORT=3306

DB_DATABASE=nombre_de_tu_base_de_datos

DB_USERNAME=tu_usuario

DB_PASSWORD=tu_contraseña

JWT (si usas JWT):

JWT_SECRET=

Ejecuta el siguiente comando para generar un secreto para JWT:

php artisan jwt:secret


Generar la Clave de la Aplicación

Genera una clave única para tu aplicación:
php artisan key:generate

5. Migrar la Base de Datos

php artisan migrate

6. Correr el Servidor de Desarrollo

Inicia el servidor de desarrollo:

php artisan serve

Esto levantará el backend en http://localhost:8000.

Comandos Importantes del Backend
Generar JWT Secret (si usas JWT):

php artisan jwt:secret

Migrar Base de Datos:
php artisan migrate

Correr Servidor de Desarrollo:
php artisan serve

Instalar Dependencias de Frontend (si usas Laravel Mix para Vue/React):
npm install
