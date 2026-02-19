# DataTrain Corp

## Bases de Datos Fullstack

Este repositorio contiene la solución al simulacro de desempeño para la gestión de entrenamientos técnicos, integrando arquitecturas relacionales (SQL) y no relacionales (NoSQL).

---

## 📊 Arquitectura del Sistema

El proyecto se basa en una arquitectura **Fullstack SPA** conectada a un entorno de base de datos híbrido.

### Stack Tecnológico

* **Frontend:** Vite + JavaScript (Vanilla/React/Vue) + CSS3.
* **Backend:** Node.js + Express.
* **Base de Datos Relacional:** MySQL / PostgreSQL (Consultas complejas y Vistas).
* **Base de Datos NoSQL:** MongoDB (Logs y Feedback).
* **ORM/Query Builders:** `mysql2`, `pg` o `knex.js` (Prohibido el uso de Sequelize/Prisma).

---

## 🗂️ Estructura del Proyecto

```bash
├── backend/              # Servidor Node.js y API REST
├── frontend/             # Código fuente de la interfaz (Vite)
├── sql/                  # Scripts de creación de tablas, semillas y vistas
│   └── database.sql      
├── mongo/                # Esquemas y ejemplos de colecciones
│   └── collections.json  
├── docs/                 # Documentación técnica
│   └── DER.png           # Diagrama Entidad-Relación (Obligatorio)
└── README.md             # Guía del proyecto

```

## 🧠 Diseño

[Haz clic aquí para ver el diseño en Figr](https://app.figr.design/artifacts/2b4955ab-606f-45f3-9b1d-00b1fa5341bb)

---

## 🛠️ Configuración e Instalación

### 1. Requisitos Previos

* Node.js (v18+)
* MySQL o PostgreSQL
* MongoDB

### 2. Base de Datos (SQL)

Importa el archivo situado en `/sql/database.sql` en tu gestor de bases de datos para crear las tablas y las vistas obligatorias:

* `v_employee_performance`
* `v_training_stats`

### 3. Variables de Entorno

Crea un archivo `.env` en la carpeta `/backend` con los siguientes datos:

```env
PORT=3000
DB_HOST=localhost
DB_USER=tu_usuario
DB_PASS=tu_contraseña
DB_NAME=datatrain_db
MONGO_URI=mongodb://localhost:27017/datatrain_nosql

```

### 4. Instalación

```bash
# Instalar dependencias del Backend
cd backend
npm install

# Instalar dependencias del Frontend
cd ../frontend
npm install

```

---

## 🚀 Funcionalidades Implementadas

### Consultas SQL de Alto Rendimiento

El sistema expone endpoints para reportes complejos que incluyen:

* **Ranking de desempeño:** Top 5 empleados con mejor promedio.
* **Análisis de capacidad:** Entrenamientos con más inscritos y entrenamientos vacíos.
* **Seguimiento:** Sesiones filtradas por rango de fechas y última sesión por curso.

### Integración NoSQL (MongoDB)

* **Feedback:** Registro de comentarios y valoraciones de empleados sobre los cursos.
* **Logs:** Trazabilidad de acciones administrativas (Auditoría).

### Interfaz de Usuario (Frontend)

* **Dashboard:** Métricas clave en tiempo real.
* **Gestión (CRUD):** Control total sobre Empleados y Entrenamientos.
* **Módulo de Reportes:** Visualización interactiva de las Vistas SQL.

---

## 📝 Criterios de Entrega

Para que el proyecto sea evaluado, debe contener:

1. **DER completo** en `/docs/DER.png`.
2. **Scripts SQL** con `JOIN`, `GROUP BY` y `Subconsultas`.
3. **Endpoints** que conecten cada consulta SQL con una vista en el Frontend.
4. **Validaciones** tanto en cliente como en servidor.

---

## 👤 Autor

* **Coder:** [GABRIELA RINCON]
* **Clan:** Hamilton
* **Fecha:** Febrero 2026
