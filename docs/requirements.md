# Functional requirements

- **FR-01 — Registration:** Visitors can register as freelancers or clients with validated input.
- **FR-02 — Authentication:** Registered users can securely log in and log out.
- **FR-03 — Job posting:** Clients can create, edit, publish, and close job listings.
- **FR-04 — Search and filtering:** Freelancers can search available jobs by title, category, and budget.
- **FR-05 — Bidding:** Freelancers can submit a proposal containing price, deadline, and cover message.
- **FR-06 — Award job:** Clients can view bids and select one freelancer per job.
- **FR-07 — Dashboard:** Users can see their job posts, applications, and statuses.
- **FR-08 — Reviews:** After completion, both sides can leave ratings and reviews.
- **FR-09 — Administration:** Administrators can moderate users and listings.

## Nonfunctional requirements

Responsive interface, consistent navigation, secure access control, server-side form validation, database persistence, useful error messages, and automated tests.

## User story example

As a freelancer, I want to filter open jobs and submit my price and proposed deadline, so that a client can consider hiring me. As a client, I want to view competing proposals and approve only one, so that the project can begin.

## Main entities

User, Category, JobOrder (Order), Bid, Review.
