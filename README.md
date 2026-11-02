# FreelanceKZ — Student Freelance Marketplace

**Laboratory Work 7 | Development of Web Applications in Java Spring | Final Exam Project Planning and UX/UI Design**

FreelanceKZ is a proposed web platform connecting students and beginning specialists with clients who need affordable digital services. Clients publish jobs; freelancers find tasks and submit bids specifying their price and deadline. After assignment completion, participants can leave ratings and reviews.

> **Project status:** Planning and UX/UI design only. The Java Spring Boot application will be implemented for the Final Exam; no working backend or payment system is claimed in this repository.

## Project materials

| Deliverable | Link |
| --- | --- |
| Project proposal (description, goals, users, expected results) | [docs/project-proposal.md](docs/project-proposal.md) |
| UX/UI design — 9 screens and navigation | [Figma design](https://www.figma.com/design/x45moe42CMHbzgNk8wAyHU) |
| UX/UI screens and main user flow | [docs/ux-ui.md](docs/ux-ui.md) |
| Functional requirements | [docs/requirements.md](docs/requirements.md) |
| Spring Boot architecture and data model | [docs/architecture.md](docs/architecture.md) |
| Technology stack and dependencies | [docs/technology-stack.md](docs/technology-stack.md) |
| Team roles | [docs/team.md](docs/team.md) |
| Development roadmap | [docs/roadmap.md](docs/roadmap.md) |
| Defense notes | [docs/presentation-guide.md](docs/presentation-guide.md) |

The formatted **PDF proposal** is prepared separately for submission. Add it under `docs/` using GitHub's **Add file → Upload files** option if the lecturer requires the PDF to be inside the repository.

## Proposed features

1. Register and log in as a client or freelancer.
2. Clients create and manage freelance job listings.
3. Freelancers browse, search and filter job listings.
4. Freelancers submit bids with proposed price, delivery date and cover message.
5. Clients review bids and assign a freelancer.
6. Users track projects and applications in a personal dashboard.
7. Clients and freelancers leave reviews after completed projects.
8. Administrators moderate users and listings.

## Selected stack

`Java 21` · `Spring Boot` · `Spring MVC` · `Thymeleaf` · `HTML / CSS / JavaScript` · `PostgreSQL` · `Spring Data JPA / Hibernate` · `Spring Security` · `Maven` · `GitHub`

**Architecture:** Frontend → Controller → Service → Repository → PostgreSQL.

**Entities:** User, Category, JobOrder (Order), Bid, Review.

## Team

| Student | Main role |
| --- | --- |
| Saduakas Bakdaulet | Backend — Spring Boot, security, orders, bids |
| Kopbolsyn Dinmukhamed | UX/UI and frontend — Figma, Thymeleaf, HTML/CSS |
| Raimkhanov Alibek | Database and integration — PostgreSQL, JPA, filtering, reviews, tests |

Every student will explain the architecture and participate in the Final Exam presentation.

## Lab 7 checklist

- [x] Project description (150–250 words), objectives, users, functional requirements, expected results
- [x] Nine UX/UI screens (minimum five)
- [x] Figma design file and prototype links between key screens
- [x] Technology stack and justified Spring Boot dependencies
- [x] Layered architecture diagram and proposed database entities
- [x] Team members and individual responsibilities
- [x] Eight-stage implementation roadmap
- [x] GitHub repository
- [ ] Verify the end-to-end Figma prototype before submitting
- [ ] Add the formatted PDF to this repository (optional unless teacher requires)
- [ ] Prepare and rehearse the oral presentation

**This repository contains planning documents, not the finished application.**
