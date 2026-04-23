# 🎬 Cinema Management System (CMS)

A scalable backend application for managing a cinema system, built with **Spring Boot** following **Hexagonal Architecture (Ports & Adapters)** principles.

---

##  Features

*  Movie management (CRUD operations)
*  Seat and hall management
*  Session scheduling
*  Reservation system
*  Customer & subscribed customer handling
*  Filtering & querying capabilities
*  Clean architecture (Domain-driven design)

---

##  Architecture

This project follows **Hexagonal Architecture (Ports & Adapters)**:

* **Domain Layer** → Entities & business logic
* **Application Layer** → Services & use cases
* **Adapters Layer** → REST controllers & DTOs
* **Infrastructure Layer** → Database interaction

This ensures:

* High testability
* Separation of concerns
* Scalability

---

##  Tech Stack

* **Backend:** Spring Boot
* **Language:** Java
* **Database:** PostgreSQL
* **ORM:** JPA / Hibernate
* **Build Tool:** Maven
* **Architecture:** Hexagonal Architecture
* **Containerization:** Docker (optional)

---

##  Project Structure

```
src/main/java/com/backend
│
├── domain
│   ├── entities
│   └── repository
│
├── application
│   └── services
│
├── adapters
│   └── in
│       └── controllers
│       └── rest
│           ├── dto
│           ├── mapper
│
└── exceptions
```

---

##  Installation & Run

### 1. Clone the repository

```bash
git clone https://github.com/Mumtaz203/CMS.git
cd CMS
```

### 2. Configure database

Edit:

```
src/main/resources/application.properties
```

Example:

```
spring.datasource.url=jdbc:postgresql://localhost:5432/cms
spring.datasource.username=postgres
spring.datasource.password=postgres

```

---

### 3. Run the application

Using Maven wrapper:

```bash
./mvnw spring-boot:run
```

Or:

```bash
mvn spring-boot:run
```

---

##  API Endpoints (Examples)

| Resource     | Endpoint        |
| ------------ | --------------- |
| Movies       | `/movies`       |
| Customers    | `/customers`    |
| Reservations | `/reservations` |
| Sessions     | `/sessions`     |
| Halls        | `/halls`        |
| Seats        | `/seats`        |

---

##  Testing

```bash
./mvnw test
```

---

##  Future Improvements

* Authentication & authorization (Spring Security)
* Swagger / OpenAPI documentation
* CI/CD pipeline (GitHub Actions)
* Frontend integration (React / Flutter)

---

##  Author

**Mümtaz Erdogan**

*  [mitaserdogan@gmail.com](mailto:mitaserdogan@gmail.com)
*  https://github.com/Mumtaz203
*  [umutavci03@gmail.com](mailto:umutavci03@gmail.com)
*  https://github.com/UmutVci

---

##  License

This project is for educational purposes.

