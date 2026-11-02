# Technology stack and required dependencies

| Component | Chosen technology | Why it is needed |
| --- | --- | --- |
| Language | Java 21 | Core object-oriented backend language, modern LTS release |
| Backend | Spring Boot | Simplifies web application configuration and development |
| Web layer | Spring MVC / Spring Web | Handles HTTP requests, controllers, and page routing |
| Frontend | Thymeleaf + HTML, CSS, JavaScript | Server-rendered forms and responsive interactive pages |
| Database | PostgreSQL | Stores relational users, job orders, bids, categories, and reviews |
| Persistence | Spring Data JPA / Hibernate | Maps Java entities and relationships to database tables |
| Authentication | Spring Security | Login, password protection, and client/freelancer/admin authorization |
| Validation | Jakarta Bean Validation via Spring Validation | Validates registration, orders, and bid forms |
| Build system | Maven | Dependency management and repeatable builds |
| Version control | Git / GitHub | Team collaboration, commits and project history |
| Testing | Spring Boot Starter Test (JUnit), Postman | Unit/integration tests and manual HTTP testing |

## Spring Boot dependencies

- **Spring Web:** Spring MVC controllers and HTTP endpoints.
- **Thymeleaf:** HTML templates with data provided by controllers.
- **Spring Data JPA:** repository interfaces, relational entity persistence.
- **PostgreSQL Driver:** connects the application to PostgreSQL.
- **Spring Validation:** validates client and freelancer input.
- **Spring Security:** login, authorization, and route protection.
- **Spring Boot Starter Test:** supports automated application testing.
- **Lombok (optional):** avoids repetitive getters/setters, if the team opts to use it.

## Communication

The browser sends HTTP GET/POST requests to Spring MVC controllers. Controllers invoke services. Services enforce business rules and call Spring Data JPA repositories. Repositories read or write PostgreSQL. Controllers return Thymeleaf views populated with model data. JavaScript is reserved for optional browser-side interactions.

No REST API or React is required by this initial design; it can be added in a future iteration.
