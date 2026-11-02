# Spring Boot application architecture

```mermaid
flowchart TD
  F[Browser / Thymeleaf / HTML CSS JS] --> C[Controller: Spring MVC]
  C --> S[Service: business logic]
  S --> R[Repository: Spring Data JPA]
  R --> DB[(PostgreSQL database)]
  SEC[Spring Security] -.protects.-> C
  E[Entity / Model] -.maps domain objects.-> R
```

## Responsibilities

- **Frontend:** Displays pages and sends HTML form requests.
- **Controller:** Receives HTTP requests and returns Thymeleaf views or redirects.
- **Service:** Applies business logic such as ensuring a job has at most one accepted bid.
- **Repository:** Queries and persists data using Spring Data JPA / Hibernate.
- **Entity / Model:** Represents application data and relational mappings.
- **Database:** PostgreSQL stores registered users, job posts, bids, and reviews.
- **Security:** Spring Security protects pages and role-specific actions.

## Entity relationships

```mermaid
erDiagram
  USER ||--o{ JOB_ORDER : creates
  CATEGORY ||--o{ JOB_ORDER : categorizes
  USER ||--o{ BID : submits
  JOB_ORDER ||--o{ BID : receives
  USER ||--o{ REVIEW : authors
  USER ||--o{ REVIEW : receives
  JOB_ORDER ||--o{ REVIEW : has
```

Example domain model:

- **User:** id, fullName, email, passwordHash, role.
- **Category:** id, name.
- **JobOrder:** id, clientId, categoryId, title, description, budget, deadline, status.
- **Bid:** id, orderId, freelancerId, proposedPrice, proposedDeadline, message, status.
- **Review:** id, orderId, authorId, recipientId, rating, comment.

## Data flow example

1. A freelancer submits a bid from a Thymeleaf form.
2. `BidController` receives the POST request and validates the input.
3. `BidService` checks that the user is authorized and that the job accepts bids.
4. `BidRepository` saves the bid entity.
5. PostgreSQL persists it and the controller redirects to the dashboard.

The architecture diagram is a planned design; Spring Boot source code is not implemented during Lab 7.
