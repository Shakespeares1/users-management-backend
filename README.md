# Gestión de Usuarios - Backend Spring Boot

## Descripción

API REST desarrollada con Spring Boot siguiendo principios de Arquitectura Hexagonal para la gestión de usuarios.

La aplicación permite realizar operaciones CRUD sobre usuarios almacenados en MySQL.

## Tecnologías Utilizadas

* Java 17
* Spring Boot 3
* Maven
* MySQL
* Swagger
* Arquitectura Hexagonal

## Funcionalidades

* Crear usuarios.
* Consultar usuarios.
* Actualizar usuarios.
* Eliminar usuarios.
* Documentación automática mediante Swagger.

## Configuración Base de Datos

Crear la base de datos:

```sql
CREATE DATABASE crud_usuarios;
```

Configurar credenciales en:

```text
src/main/resources/application.properties
```

Ejemplo:

```properties
db.host=localhost
db.port=3306
db.name=crud_usuarios
db.username=root
db.password=TU_PASSWORD
```

## Ejecución

Clonar repositorio:

```bash
git clone https://github.com/Shakespeares1/users-management-backend.git
```

Ingresar al proyecto:

```bash
cd users-management-backend
```

Ejecutar:

```bash
mvn spring-boot:run
```

## Swagger

Disponible en:

```text
http://localhost:8080/swagger-ui/index.html
```

## Endpoints

| Método | Endpoint        |
| ------ | --------------- |
| GET    | /api/users      |
| GET    | /api/users/{id} |
| POST   | /api/users      |
| PUT    | /api/users/{id} |
| DELETE | /api/users/{id} |

## Arquitectura

El proyecto implementa Arquitectura Hexagonal mediante:

* Domain
* Application
* Infrastructure

## Autor

Antonio De Ávila
Universidad de Cartagena
Desarrollo Web
