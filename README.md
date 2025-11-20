# 📚 Proyecto Backend: API de Gestión de Libros y Autores

Este proyecto tiene como objetivo desarrollar una API RESTful para la gestión de una biblioteca simple, enfocándose en el manejo de relaciones de datos "uno a muchos", una habilidad fundamental para cualquier desarrollador backend.

---

## 🎯 Objetivo Principal

Implementar una API que maneje dos entidades principales (Autor y Libro) y que refleje su relación jerárquica en la base de datos y a través de los endpoints.

---

## ⚙️ Requerimientos Técnicos

### 1. Modelos de Datos

El sistema debe manejar dos modelos clave con una relación estricta:

| Modelo Clave | Relación |
| :--- | :--- |
| *Autor (Author)* | Un *Autor* puede tener *muchos Libros*. |
| *Libro (Book)* | Cada *Libro* debe tener *un solo Autor*. |

### 2. Base de Datos

* *Persistencia:* La API debe conectarse a una base de datos relacional o NoSQL de su elección.
* *Opciones Sugeridas:* MySQL, PostgreSQL, MariaDB, OracleDB, o MongoDB.
* *Habilidad Clave:* Se debe manejar correctamente las *claves foráneas* (Foreign Keys) o referencias para asegurar la integridad de la relación uno a muchos.

### 3. Endpoints de la API

El proyecto debe exponer los siguientes endpoints RESTful:

| Recurso | Método HTTP | Ruta | Descripción |
| :--- | :--- | :--- | :--- |
| *Autor* | POST, GET, PUT, DELETE | /authors, /authors/{id} | Implementación *CRUD* completa para la gestión de Autores. |
| *Libro* | POST, GET, PUT, DELETE | /books, /books/{id} | Implementación *CRUD* completa para la gestión de Libros. |
| *Anidado* | GET | /authors/{author_id}/books | *Obtener todos los libros* asociados a un autor específico (author_id). |

### 4. Tecnologías y Lenguaje

El desarrollador tiene total libertad para elegir el stack que prefiera para su implementación:

* *Lenguaje de Programación:* El que le resulte más cómodo.
* *Frameworks Sugeridos:*
    * *Java* con *Spring Boot*.
    * *Node.js* con *Express* (o frameworks similares como NestJS).

---

## ✨ Habilidades a Demostrar

Este proyecto está diseñado para validar las siguientes habilidades esenciales de un desarrollador backend Junior:

1.  *Modelado de Datos:* Definir y aplicar relaciones *uno a muchos* en la base de datos.
2.  *Manejo de ORM/Conexión:* Configurar y utilizar herramientas para interactuar con la base de datos (como JPA, Sequelize, Mongoose, etc.).
3.  *Diseño RESTful:* Implementar endpoints *anidados* para consultas específicas (/authors/{id}/books).
4.  *Integridad de Datos:* Asegurar que los libros no puedan existir sin una referencia válida a un autor.
