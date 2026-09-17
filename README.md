# API REST de Usuarios

API REST desarrollada con **Java 17 + Spring Boot 3** para listar usuarios desde una base de datos H2 en memoria.

##  Tecnologías

- Java 17
- Spring Boot 3.2.5
- Spring Web
- Spring Data JPA
- H2 Database
- Maven

## 📂 Arquitectura en capas

```
controller → service → repository → model
```

## ▶️ Cómo ejecutar

```bash
./mvnw spring-boot:run
```

En Windows:

```bash
mvnw.cmd spring-boot:run
```

## 🔗 Endpoints

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| GET | `/api/usuarios` | Lista todos los usuarios |
| GET | `/api/usuarios/{id}` | Obtiene un usuario por ID |

### Ejemplo `GET /api/usuarios`

```json
[
  { "id": 1, "nombre": "Ana Pérez", "email": "ana@mail.com", "edad": 25 },
  { "id": 2, "nombre": "Luis Gómez", "email": "luis@mail.com", "edad": 30 },
  { "id": 3, "nombre": "María Ruiz", "email": "maria@mail.com", "edad": 28 }
]
```

## 🧪 Probar

- Navegador: http://localhost:8080/api/usuarios
- Consola H2: http://localhost:8080/h2-console
  - JDBC URL: `jdbc:h2:mem:usuariosdb`
  - Usuario: `sa`, sin password

## 📸 Capturas

 <img width="920" height="229" alt="image" src="https://github.com/user-attachments/assets/ab21171b-5fda-49d9-bc7b-de30285d42bc" />
 <img width="920" height="466" alt="image" src="https://github.com/user-attachments/assets/4677f10c-103c-4079-b96e-bbfb7407902a" />


