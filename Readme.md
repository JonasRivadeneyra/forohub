<a id="readme-inicio"></a>

<div align="center">

![java](https://img.shields.io/badge/Java-17.0.12-red)
![spring](https://img.shields.io/badge/Spring-3.3.5-red)
![hibernate](https://img.shields.io/badge/Hibernate-6.5.3-red)
![mysql](https://img.shields.io/badge/MySQL-8.0.40-red)
![flyway](https://img.shields.io/badge/Flyway-10.10.0-red)
![auth0jwt](https://img.shields.io/badge/Auth0JWT-4.4.0-red)
![lombok](https://img.shields.io/badge/Lombok-1.18.34-red)
![springdoc](https://img.shields.io/badge/SpringDoc-2.6.0-red)
![intellij](https://img.shields.io/badge/IntelliJ-CE%202024.2.2-red)
</div>

<div align="center">

![license](https://img.shields.io/badge/License-0BSD-brightgreen)
![update](https://img.shields.io/badge/Update-18%2FAug%2F2025-blue)
![version](https://img.shields.io/badge/Version-1.0.0-blue)
![stage](https://img.shields.io/badge/Stage-Release-blue)

</div>

# ForoHub

## Índice
- [Contexto](#contexto)
- [Teoría del Proyecto](#teoria-del-proyecto)
- [Guía de Usuario](#guía-de-usuario)
- [Guía de Instalación](#guía-de-instalación)
- [Licencia](#licencia)
- [Agradecimientos](#agradecimientos)
- [Documentos Complementarios](#documentos-complementarios)

---

## Contexto
ForoHub es una aplicación desarrollada en Java con IntelliJ para el desafío del curso *“Practicando Spring Framework: Challenge Foro Hub”* de ONE + Alura Latam, publicada el 18 de agosto de 2025.

---

## Teoría del Proyecto
En esta clase se construye una **API REST para un foro** usando **Java y Spring Boot**.

**Puntos clave:**
- **Creación de la API:** Usuarios pueden crear tópicos con dudas o sugerencias, y otros pueden responder.
- **Pruebas con Insomnia:** Se usa Insomnia para probar endpoints sin interfaz gráfica.
- **Endpoints principales:**
    - `GET /tópicos`: Lista todos los tópicos.
    - `POST /tópicos`: Crea un nuevo tópico (requiere autenticación).
    - `POST /auth`: Autenticación y obtención de token JWT.
    - `DELETE /tópicos/{id}`: Elimina un tópico (requiere autenticación).
- **Seguridad:** Tokens JWT protegen creación, eliminación y actualización de tópicos.
- **Flujo de autenticación:** `/auth` recibe email y contraseña, genera token Bearer para endpoints protegidos.
- **Status Codes:** Uso correcto de códigos HTTP (200 OK, 201 Created, 403 Forbidden).
- **Herramienta Trello:** Para dividir el proyecto en tareas pequeñas y gestionables.
- **Personalización:** Se anima a los estudiantes a añadir funcionalidades y estilo propio al foro.

---

## Guía de Usuario
API REST con CRUDs completos para **tópicos** y **usuarios**.

- Interfaz accesible vía **SpringDoc-Swagger**:  
  http://localhost:8080/swagger-ui/index.html
- Requests disponibles en archivo importable en **Insomnia**.
- Autenticación con **Auth0-JWT** y contraseñas encriptadas con **Bcrypt**.
- Base de datos gestionada mediante **Flyway** para migraciones.

---

## Guía de Instalación
1. Clonar el proyecto localmente.
2. Ejecutar desde el método `main` de `ForoHubApplication` en IntelliJ o Eclipse.
3. Requerimientos: **MySQL 8.0.40+** y declarar variables de entorno en `application.properties`.
4. Scripts SQL para pruebas incluidos en el repositorio.

---


## Agradecimientos
- Generador de logotipo: https://chatgpt.com
- Generador de favicon: https://favicon.io

---

## Documentos Complementarios
- [Clonar un repositorio de GitHub](https://docs.github.com/es/repositories/creating-and-managing-repositories/cloning-a-repository)
- [Scripts SQL para pruebas](https://github.com/cesargh/forohub/tree/master/sql)
- [Requests de Insomnia](https://github.com/cesargh/forohub/tree/master/insomnia)  
