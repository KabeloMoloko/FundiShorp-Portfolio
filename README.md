# FundiShorp — Agile Software Development Portfolio

**Project:** FundiShorp  
**Project Type:** Home Improvement Marketplace Web Application  
**Methodology:** Agile Scrum  
**Project Management Tool:** Trello  
**Frontend:** React  
**Backend:** Java Spring Boot  
**Database:** MySQL  
**Cloud and Deployment:** AWS and CI/CD (as specified in the project plan)  
**Version Control:** Git and GitHub  
**Project Board:** [FundiShorp on Trello](https://trello.com/b/aviqvFPS/fundishorp)  
**Project Status:** Development and verification of deliverables in progress

---

## Table of Contents

- [1. Project Overview](#1-project-overview)
- [2. Agile Project Charter](#2-agile-project-charter)
- [3. Scope and Requirements](#3-scope-and-requirements)
- [4. Stakeholders and Team Roles](#4-stakeholders-and-team-roles)
- [5. Agile Methodology](#5-agile-methodology)
- [6. User Stories and Tasks](#6-user-stories-and-tasks)
- [7. Product Backlog](#7-product-backlog)
- [8. Sprint Backlog](#8-sprint-backlog)
- [9. Sprint Schedule and Milestones](#9-sprint-schedule-and-milestones)
- [10. Agile Logbook](#10-agile-logbook)
- [11. Definition of Ready and Definition of Done](#11-definition-of-ready-and-definition-of-done)
- [12. Testing and Quality Assurance](#12-testing-and-quality-assurance)
- [13. Risk Management](#13-risk-management)
- [14. GitHub and Trello Project Organisation](#14-github-and-trello-project-organisation)
- [15. Agile Reflection Using STAR](#15-agile-reflection-using-star)
- [16. Conclusion](#16-conclusion)
- [17. References](#17-references)

---

# 1. Project Overview

## 1.1 Introduction

FundiShorp is a proposed home-improvement marketplace that connects homeowners with fundis, including tradespeople who provide services and sell building materials.

The platform is intended to allow homeowners to discover verified fundis, browse product listings, compare labour and callout rates, purchase materials, book jobs, and review completed work.

Fundis can register for trade accounts, create storefronts, manage product listings, publish service rates, respond to booking requests, and build their reputations through customer reviews.

Administrators are responsible for platform oversight, including reviewing verification documents, managing user access, monitoring transactions, and addressing fraudulent storefronts.

The project uses Agile Scrum principles to organise development into manageable increments. Trello is used to track the product backlog, sprint work, tasks, and development progress.

## 1.2 Problem Statement

Homeowners may struggle to find trustworthy tradespeople, compare service rates, obtain building materials, and coordinate a job with a suitable fundi.

Fundis may also lack a centralised digital platform through which they can promote their services, sell materials, manage bookings, and establish trust with potential customers.

FundiShorp aims to address these problems by combining tradesperson discovery, product listings, transparent pricing, job booking, and trust-related features in one marketplace.

## 1.3 Project Aim

The aim is to develop a secure, accessible, and maintainable home-improvement marketplace that enables homeowners to discover fundis, purchase materials, book services, and manage the main stages of a job.

## 1.4 Project Objectives

The project objectives are to:

1. Develop a React frontend connected to a Java Spring Boot backend.
2. Design and implement a MySQL database with appropriate relationships and constraints.
3. Provide registration and login for homeowners and fundis.
4. Implement role-based access for homeowners, fundis, and administrators.
5. Enable fundis to submit verification documents and create storefronts.
6. Allow fundis to manage product and material listings.
7. Display transparent material, labour, and callout pricing.
8. Support searching for fundis by trade category and location.
9. Provide a shopping cart that supports materials and booking-related items.
10. Support booking requests and fundi responses.
11. Implement payment, escrow, commission, and order-confirmation workflows where supported.
12. Allow customers to review completed jobs.
13. Provide administrative monitoring and trust-and-safety functions.
14. Apply testing, version control, documentation, and continuous improvement throughout development.

## 1.5 Target Users

| User | Description | Main requirements |
|---|---|---|
| Homeowner | A customer seeking services or materials | Search, compare, buy, book, pay, and review |
| Fundi | A tradesperson offering services or materials | Register, verify, manage storefront, set rates, and handle bookings |
| Administrator | A person responsible for platform oversight | Verify fundis, manage permissions, monitor activity, and handle abuse |
| Platform business | The operator of FundiShorp | Manage commissions, subscriptions, booking fees, and revenue reports |

## 1.6 Value Proposition

FundiShorp aims to provide:

- **Convenience:** Access to services and materials through one platform.
- **Trust:** Verification, ratings, reviews, and administrative oversight.
- **Transparency:** Published product prices, labour rates, and callout fees.
- **Coordination:** Booking requests, status updates, and job completion.
- **Business opportunities:** Digital storefronts and revenue opportunities for fundis.

---

# 2. Agile Project Charter

## 2.1 Charter Summary

| Charter item | Description |
|---|---|
| Project name | FundiShorp |
| Project category | Home-improvement marketplace |
| Project methodology | Agile Scrum |
| Product Owner | To be formally confirmed by the team |
| Scrum Master | To be formally confirmed by the team |
| Development team | FundiShorp student project team |
| Stakeholders | Homeowners, fundis, administrators, and academic stakeholders |
| Project management | Trello |
| Version control | GitHub |
| Frontend technology | React |
| Backend technology | Java Spring Boot |
| Database technology | MySQL |
| Planned deployment | AWS with CI/CD |
| Project roadmap | 13 sprint stages recorded on Trello |

## 2.2 Project Vision

To provide a trusted digital marketplace where homeowners can find skilled tradespeople, purchase materials, compare prices, book services, and manage home-improvement jobs while helping fundis promote and grow their businesses.

## 2.3 Business Justification

FundiShorp addresses the need for a more organised way to discover tradespeople and coordinate home-improvement work.

The platform brings together functions that would otherwise require customers to use separate services, such as finding a tradesperson, comparing prices, buying materials, arranging a job, and reviewing the service received.

The project also provides a practical opportunity to apply software engineering, database design, secure application development, Agile project management, and collaborative version control.

## 2.4 Project Scope

### In scope

- Homeowner and fundi registration and login.
- Role-based access control.
- Fundi verification and approval workflows.
- Fundi storefront creation and management.
- Product and material listing management.
- Product details, images, and pricing.
- Labour rates and callout fees.
- Search by trade category and location.
- Search filtering and sorting.
- Shopping cart and checkout.
- Materials-only purchasing.
- Combined materials and booking checkout.
- Job booking and scheduling.
- Booking acceptance, decline, and rescheduling.
- Job completion and payment workflow.
- Payment handling and escrow-related logic.
- Platform commissions and booking fees.
- Ratings and reviews.
- Customer profiles and fundi verification status.
- Administrative dashboard and trust-and-safety controls.
- Notifications.
- Revenue reporting.
- Testing, documentation, deployment, and final demonstration.

### Out of scope for the initial agreed roadmap

The following are not explicitly established as initial deliverables on the supplied board and should require separate approval:

- Native Android and iOS applications.
- International marketplace expansion.
- Advanced AI-based matching of homeowners and fundis.
- Complex enterprise accounting integrations.
- Automated dispute resolution using artificial intelligence.
- Additional payment providers not included in the approved design.

## 2.5 Assumptions

- Team members have access to the Trello board and GitHub repository.
- The team can work with React, Java Spring Boot, and MySQL.
- Required development tools and testing environments are available.
- Payment and deployment integrations can be configured using suitable credentials and environments.
- The team will maintain documentation and update task statuses throughout development.
- Security and privacy requirements will be considered during implementation.

## 2.6 Constraints

- Limited academic project time.
- Dependencies between the database, backend, and frontend.
- Integration complexity for authentication, payments, and booking workflows.
- External service requirements for cloud hosting and payment processing.
- The need to balance implementation with testing and documentation.
- The large scope represented by 13 planned sprint stages.

## 2.7 Success Criteria

FundiShorp will be evaluated against the following criteria:

1. Users can register and access the correct role-specific features.
2. Fundis can submit verification information and manage storefronts.
3. Customers can browse listings and view relevant prices.
4. Customers can search for fundis and create booking requests.
5. Cart and checkout calculations are correct.
6. The booking lifecycle follows the agreed status transitions.
7. Payment-related workflows are tested safely in the intended environment.
8. Reviews are restricted to eligible completed jobs.
9. Administrative functions enforce appropriate permissions.
10. Critical security and data-integrity defects are addressed.
11. Source code and project documentation are maintained in GitHub.
12. Trello accurately reflects the work completed and remaining.

---

# 3. Scope and Requirements

## 3.1 Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR01 | Register and authenticate homeowners | Must have |
| FR02 | Register fundis and create trade accounts | Must have |
| FR03 | Enforce role-based access | Must have |
| FR04 | Submit and review verification documents | Must have |
| FR05 | Create and manage fundi storefronts | Must have |
| FR06 | Create, edit, and remove material listings | Must have |
| FR07 | Display product information, images, and prices | Must have |
| FR08 | Set labour and callout rates | Must have |
| FR09 | Search for verified fundis by category and location | Must have |
| FR10 | Add materials to a cart | Must have |
| FR11 | Support materials-only checkout | Must have |
| FR12 | Support booking requests and responses | Must have |
| FR13 | Support combined materials and booking checkout | Should have |
| FR14 | Handle order and payment confirmation | Must have |
| FR15 | Support job completion and escrow release rules | Must have |
| FR16 | Allow eligible customers to rate and review fundis | Should have |
| FR17 | Provide an administrative dashboard | Should have |
| FR18 | Support profiles, filters, and sorting | Should have |
| FR19 | Provide platform revenue features and reporting | Could have |
| FR20 | Provide booking and order notifications | Should have |

The priorities are proposed from the roadmap and should be confirmed by the Product Owner. They do not replace the team's official prioritisation decisions.

## 3.2 Non-Functional Requirements

### Security
- Passwords must be stored using an appropriate password-hashing mechanism.
- Protected operations must enforce backend authorisation.
- Sensitive data must not be exposed through error messages or logs.
- Payment handling must use an appropriate compliant payment provider.
- Uploaded documents must be protected from unauthorised access.

### Performance
- Search and listing queries should respond within agreed performance targets.
- Database queries should avoid unnecessary repeated requests.
- The application should remain usable under expected demonstration workloads.

### Reliability
- Booking status changes must be consistent.
- Cart totals must be calculated correctly.
- Duplicate payment or order submissions must be handled safely.
- Database relationships and constraints must preserve transactional integrity.

### Usability
- Forms should provide clear validation feedback.
- Pricing should be displayed transparently.
- Users should understand booking and order statuses.
- Pages should adapt to desktop, tablet, and mobile screens.

### Maintainability
- The backend should follow the planned layered architecture.
- Frontend components should be reusable.
- The project should use version control and meaningful commits.
- Documentation should be updated as features change.

---

# 4. Stakeholders and Team Roles

## 4.1 Project Team

The exported Trello board identifies the following members.

| Team member | Project participation |
|---|---|
| Kabelo Nimrod Moloko | Team member |
| Christian Hakizimana | Team member |
| Lisakhanya Mpahla | Team member |

The board contains task assignments, but the project-wide roles below should be confirmed by the team rather than assumed from membership alone.

## 4.2 Proposed Agile Roles

| Role | Responsibilities |
|---|---|
| Product Owner | Maintains the product vision, clarifies requirements, and prioritises stories |
| Scrum Master | Facilitates Scrum activities and helps remove blockers |
| Frontend Developer | Builds React pages, components, routing, and API integration |
| Backend Developer | Builds Spring Boot services, business logic, and REST endpoints |
| Database Developer | Designs MySQL entities, relationships, and constraints |
| Quality Assurance | Creates test scenarios, records defects, and verifies fixes |
| DevOps Coordinator | Manages deployment configuration and CI/CD |
| Documentation Coordinator | Maintains the README, logbook, and project evidence |

Team members may perform multiple roles. Assign an owner to every active Trello card so that responsibility is clear.

---

# 5. Agile Methodology

## 5.1 Why Agile Scrum?

Scrum supports incremental delivery, regular feedback, visible work, and continuous improvement.

FundiShorp has several connected features, including registration, verification, storefronts, listings, bookings, and payments. Developing these features in stages makes it easier to identify dependencies and test functionality before building additional layers.

## 5.2 Agile Workflow

The team follows this proposed workflow:

1. Gather and clarify requirements.
2. Create and prioritise product backlog items.
3. Refine stories and define acceptance criteria.
4. Select work during sprint planning.
5. Implement the selected tasks.
6. Test the functionality.
7. Review the increment with stakeholders.
8. Record feedback and update the backlog.
9. Conduct a retrospective.
10. Apply lessons learned to the next sprint.

## 5.3 Trello Workflow

The board has the following lists:

- Product Backlog
- Sprint 1 Backlog
- Sprint 2
- Sprint 3
- Sprint 4
- Sprint 5

These lists provide a starting point for organising requirements and sprint work. The board would be easier to maintain with additional workflow lists such as:

- To Do
- In Progress
- Code Review
- Testing
- Done
- Blocked

These are recommendations, not claims that the additional lists already exist.

## 5.4 Scrum Events

### Sprint Planning
The team selects prioritised work, agrees on a sprint goal, and identifies dependencies.

### Daily Coordination
Team members communicate completed work, next steps, and blockers.

### Sprint Review
The team demonstrates working features and collects stakeholder feedback.

### Sprint Retrospective
The team identifies strengths, problems, and actions to improve the next sprint.

---

# 6. User Stories and Tasks

The user stories below are based on the FundiShorp cards in the Trello export. The tasks summarise the work described in the card checklists.

Acceptance criteria are included to make the expected results testable. Verify them with the Product Owner before treating them as formally approved.

## Epic 1: Backend Architecture and Database

### US01 — Establish the database schema

**User story:** As a developer, I want the MySQL database designed before implementing backend layers so that data relationships and transactional integrity are established early.
## Database Schema

![FundiShorp Database Schema](screenshots/databaseschema.png)

**Tasks:**
- Design the ERD for users, fundis, storefronts, listings, orders, bookings, and reviews.
- Implement the database schema and migrations.
- Configure relationships and constraints.
- Insert sample data.
- Test schema operations and queries.

**Acceptance criteria:**
- Required entities and relationships are documented.
- Foreign-key relationships are valid.
- Required constraints are enforced.
- Sample queries execute successfully.

### US02 — Build the layered backend

**User story:** As a developer, I want the backend to follow a layered Java Spring Boot architecture so that the application remains maintainable and scalable.

**Tasks:**
- Create domain classes using the Builder pattern.
- Create factories for constructing and validating domain objects.
- Implement Spring Data JPA repositories.
- Add service classes for business logic.
- Implement REST controllers.
- Test the controller-to-service-to-repository flow.

**Acceptance criteria:**
- Responsibilities are separated between layers.
- Domain objects are constructed according to the agreed pattern.
- Controllers expose the intended API operations.
- Core operations are verified through tests.

## Epic 2: Frontend Foundation and Deployment

### US03 — Establish the React frontend

**User story:** As a developer, I want a reusable React frontend with routing and API integration so that new features can be developed consistently.

**Tasks:**
- Initialise the React project.
- Configure routing and environment variables.
- Implement global state management.
- Create the API client.
- Build reusable UI components.
- Implement authentication context and protected routes.
- Test responsive layouts and backend connectivity.

**Acceptance criteria:**
- Main routes work as intended.
- Reusable components follow a consistent design.
- API calls use the configured backend.
- Protected routes enforce the agreed access rules.

### US04 — Prepare cloud deployment

**User story:** As a DevOps engineer, I want the application deployed through a repeatable process so that it can be tested and released reliably.

**Tasks:**
- Configure AWS environments.
- Set up the CI/CD pipeline.
- Configure deployment scripts.
- Manage environment variables and secrets.
- Test deployment.

**Acceptance criteria:**
- Deployment configuration is documented.
- Secrets are not committed to source control.
- The deployment process produces a verifiable result.
- Failed deployments can be diagnosed.

## Epic 3: Accounts and Authentication

### US05 — Register and log in as a homeowner

**User story:** As a homeowner, I want to register and log in so that I can browse listings and book fundis.

**Tasks:**
- Design registration and login forms.
- Implement form validation.
- Create backend authentication endpoints.
- Connect the React forms to the backend.
- Implement secure session or token handling.
- Test registration, login, and error cases.
- Add email verification and password reset if included in the agreed scope.

**Acceptance criteria:**
- Valid registration data is accepted.
- Invalid data is rejected with clear feedback.
- Valid credentials permit login.
- Invalid credentials do not grant access.
- Passwords are not stored in plain text.

### US06 — Register as a fundi

**User story:** As a fundi, I want to register for a trade account so that I can create a storefront.

**Tasks:**
- Design the fundi registration form.
- Capture trade category and required information.
- Implement the registration endpoint.
- Support document submission.
- Connect the frontend to the backend.
- Test validation and error states.

**Acceptance criteria:**
- A fundi can submit the required information.
- Invalid submissions are rejected.
- The account has the correct role.
- Submitted documents are handled securely.

### US07 — Enforce role-based access

**User story:** As an administrator, I want role-based access control so that only authorised users can access protected functions.

**Tasks:**
- Define the homeowner, fundi, and administrator permissions.
- Implement backend role checks.
- Implement frontend route guards.
- Test authorised and unauthorised access.

**Acceptance criteria:**
- Each role can access only its permitted operations.
- Protected API endpoints enforce permissions on the server.
- Unauthorised requests are rejected.
- Access rules are covered by tests.

## Epic 4: Trade Verification and Storefronts

### US08 — Review fundi verification documents

**User story:** As an administrator, I want to review submitted identity and qualification documents so that I can approve or reject fundis.

**Tasks:**
- Create the administrator review queue.
- Implement endpoints to retrieve submitted applications.
- Add approve and reject operations.
- Notify fundis when the status changes.
- Test the complete verification workflow.

**Acceptance criteria:**
- An authorised administrator can review submissions.
- A submission can be approved or rejected.
- The status is saved correctly.
- The fundi receives appropriate status feedback.

### US09 — Display a verified badge

**User story:** As a fundi, I want a verified badge on my storefront after approval so that customers can identify verified tradespeople.

**Tasks:**
- Create the verified badge component.
- Connect badge visibility to verification status.
- Test approved and unapproved accounts.

**Acceptance criteria:**
- Approved fundis display the badge.
- Unapproved fundis do not display the badge.
- The status is derived from trusted backend data.

### US10 — Create a storefront

**User story:** As a fundi, I want to customise my storefront so that customers can learn about my business and services.

**Tasks:**
- Design the storefront layout.
- Add biography, trade category, service area, and branding.
- Implement storefront CRUD endpoints.
- Create the storefront editor.
- Test updates and image uploads.

**Acceptance criteria:**
- A fundi can create and update their storefront.
- The storefront displays the saved information.
- Invalid data is rejected.
- Only authorised users can edit the relevant storefront.

## Epic 5: Product Listings and Pricing

### US11 — Add products and materials

**User story:** As a fundi, I want to add products and materials to my storefront so that customers can purchase them.

**Tasks:**
- Create the product form.
- Implement the listing creation endpoint.
- Support product images.
- Connect the frontend to the backend.
- Validate product information.

**Acceptance criteria:**
- A fundi can create a listing.
- Listings display the correct name, price, and details.
- Invalid listing data is rejected.
- Product images are handled correctly.

### US12 — Edit and remove listings

**User story:** As a fundi, I want to edit or remove listings so that my storefront remains accurate.

**Tasks:**
- Implement edit and delete endpoints.
- Create the frontend editing controls.
- Update product stock and price where supported.
- Test the changes.

**Acceptance criteria:**
- An authorised fundi can update their listings.
- Removed listings no longer appear as available.
- Updated prices and stock are reflected in the interface.
- Unauthorised edits are rejected.

### US13 — View product details

**User story:** As a customer, I want to view product details and photos so that I can decide what to buy.

**Tasks:**
- Build the product details page.
- Display product images.
- Connect the page to the backend.
- Show price and stock information.
- Test valid and invalid product references.

**Acceptance criteria:**
- The correct product details are displayed.
- Price and availability match the saved listing.
- Missing products are handled appropriately.

### US14 — Set labour and callout rates

**User story:** As a fundi, I want to set my callout fee and hourly or job rate so that customers can see service pricing upfront.

**Tasks:**
- Design the rate-setting form.
- Implement the backend endpoint.
- Connect the frontend form to the API.
- Display the rates alongside relevant listings.
- Test saved rates.

**Acceptance criteria:**
- Fundis can update permitted rate fields.
- Rates are saved and displayed accurately.
- Invalid or negative values are rejected.
- Customers can distinguish labour charges from material costs.

### US15 — Display combined job pricing

**User story:** As a customer, I want to see labour pricing alongside material prices so that I can understand the expected job cost before booking.

**Tasks:**
- Build a combined pricing summary.
- Display material and labour amounts separately.
- Calculate the applicable total.
- Test pricing display on storefront and booking pages.

**Acceptance criteria:**
- Material and labour amounts are distinguishable.
- Totals use the correct values.
- The interface does not present unavailable fees as confirmed charges.

## Epic 6: Search and Shopping Cart

### US16 — Search for verified fundis

**User story:** As a customer, I want to search for verified fundis by trade category and location so that I can find a suitable professional nearby.

**Tasks:**
- Design search and filter controls.
- Implement the backend search endpoint.
- Display search results and verification
