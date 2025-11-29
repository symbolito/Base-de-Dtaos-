# Base-de-Datos-

📦 Base de Datos – Proyecto Gestor de Tareas

Este repositorio contiene la definición completa del modelo de datos utilizado por la aplicación Gestor de Tareas, implementado sobre PostgreSQL y desplegado en la nube mediante una instancia AWS EC2.

🚀 Contenido del repositorio
📂 1. Scripts SQL

Dentro de la carpeta /sql encontrarás:

Archivo	Descripción
01_creacion_tablas.sql	Script para crear todas las tablas del proyecto.
02_inserts.sql	Datos de prueba (mínimo 5 registros por tabla).
03_consultas.sql	Consultas SQL básicas y consultas JOIN.
04_drop.sql	Script opcional para eliminar todas las tablas.
🗂️ 2. Modelo Entidad–Relación (ERD)

En la carpeta /diagramas se encuentra el diagrama ER del proyecto, exportado desde DBeaver.

El modelo incluye:

🔹 Tabla tareas

id (PK)

texto

fecha

completada

created_at

🔹 Tabla adicional (ejemplo sugerido): categorias

id (PK)

nombre

🔹 Relación

Una categoría puede tener muchas tareas → 1:N

categorias (1) ---- (N) tareas

🌐 3. Conexión a la Base de Datos

Archivo: CONEXION.md

Incluye:

Motor utilizado: PostgreSQL

Servidor en cloud: AWS EC2 (instancia Linux)

Puertos utilizados: 5432

Cadena de conexión (sin credenciales sensibles)

Ejemplo:

postgres://USER:PASS@HOST:5432/DB_NAME

🛠️ 4. Cómo ejecutar los scripts
Crear estructura
\i sql/01_creacion_tablas.sql;

Insertar datos
\i sql/02_inserts.sql;

Consultar
\i sql/03_consultas.sql;

📌 Tecnologías utilizadas

PostgreSQL 14+

DBeaver para diseño del modelo

AWS EC2 para despliegue de servidor

Ubuntu Server como entorno

👨‍💻 Sebastian Blanco Baron 

Proyecto academico
