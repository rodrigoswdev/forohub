# ForoHub App

**ForoHub** es un sistema educativo construido con Spring Boot que permite a los usuarios crear, organizar y participar en foros, gestionando cursos, temas y respuestas de forma segura y ordenada.

---

## Características

- **Gestión de Usuarios:** Autenticación y autorización con JWT.
- **Gestión de Foros:** Crear y visualizar temas y respuestas.
- **Gestión de Cursos:** Asociar cursos con temas y categorías.
- **Seguridad:** Roles y permisos implementados con Spring Security.

---

## Arquitectura del Sistema

Se utiliza **arquitectura por capas**:

1. **Capa API:** Controladores REST y configuraciones de seguridad.
2. **Capa de Dominio:** Entidades, repositorios y DTOs.
3. **Capa de Infraestructura:** Configuración de base de datos, manejo de errores y documentación de API.

---

## Tecnologías Utilizadas

- **Lenguaje:** Java 17
- **Framework:** Spring Boot
- **Seguridad:** Spring Security, JWT
- **Acceso a Datos:** Spring Data JPA, Hibernate
- **Base de Datos:** MySQL
- **Documentación:** SpringDoc OpenAPI (Swagger)

### Configuración de Base de Datos

1. Crear una base de datos en MySQL Workbench, de preferencia.
2. Actualizar las credenciales en `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost/forohub
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña

```
## Endpoints

| Método | Endpoint    | Descripción                       |
| ------ | ----------- | --------------------------------- |
| POST   | /auth/login | Autenticar un usuario             |
| GET    | /users      | Obtener lista de usuarios         |
| GET    | /topics     | Listar todos los temas            |
| POST   | /topics     | Crear un nuevo tema               |
| GET    | /courses    | Listar todos los cursos           |
| POST   | /responses  | Publicar una respuesta en un tema |



