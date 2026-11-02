# Lab 7 presentation guide

## Speaker 1 — Bakdaulet: Project overview and backend

“Our project is FreelanceKZ, a freelance marketplace for students and beginning specialists. Clients post small projects. Freelancers browse orders and submit bids. A client can choose a suitable proposal. We plan to use Java Spring Boot, Spring MVC, and Spring Security to manage business logic and authentication.”

## Speaker 2 — Dinmukhamed: UX/UI

“We designed nine application screens in Figma, including the home page, job catalogue, job details, bid form, registration, login, dashboard, creating a job, and freelancer profile. Our main user flow moves from the catalogue to the job details and submission of a bid.”

## Speaker 3 — Alibek: Database and plan

“Our database will use PostgreSQL and Spring Data JPA. The main entities are User, Category, JobOrder, Bid, and Review. The architecture is Frontend, Controller, Service, Repository, and Database. We have an eight-stage development roadmap for the Final Exam.”

## Likely questions

**Q: Is the web application already implemented?**  
A: No. Lab 7 only requires project planning, design, architecture and roadmap.

**Q: Why Spring Boot?**  
A: It supports clear layered architecture, data persistence, web controllers, and security.

**Q: Why PostgreSQL?**  
A: The data is relational: users, orders, bids and reviews are connected.

**Q: What does the Service layer do?**  
A: It enforces business rules, such as allowing one accepted bid per project.

**Q: How does the user interact with the server?**  
A: A Thymeleaf web form sends a request to a Spring MVC controller, which calls the service and repository.
