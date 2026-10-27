
# FundiShorp — Agile Project Portfolio

**Project type:** Home Improvement Marketplace  
**Methodology:** Agile Scrum  
**Project management tool:** Trello  
**Frontend:** React  
**Backend:** Java Spring Boot  
**Database:** MySQL  
**Version control:** Git and GitHub  
**Project status:** Development and verification in progress

**Project links:** [GitHub Repository](https://github.com/KabeloMoloko/FundiShorp-Portfolio) | [Trello Board](https://trello.com/b/aviqvFPS/fundishorp)

---

## Table of Contents

1. [Agile Project Charter](#1-agile-project-charter)
2. [User Stories and Tasks](#2-user-stories-and-tasks)
3. [Product Backlog](#3-product-backlog)
4. [Sprint Backlog](#4-sprint-backlog)
5. [Agile Logbook](#5-agile-logbook)
6. [Supporting Evidence and References](#6-supporting-evidence-and-references)

---

# 1. Agile Project Charter

## 1.1 Project Overview

FundiShorp is a proposed home-improvement marketplace that connects homeowners with fundis (tradespeople) who provide services and sell building materials.

The platform aims to help homeowners find suitable tradespeople, compare prices, browse materials, book services, and review completed work. Fundis can register, create storefronts, manage listings, and respond to customer requests.

The project uses Agile Scrum to organise development into manageable increments, while Trello supports backlog management, task allocation, sprint planning, and progress tracking.

## 1.2 Problem Statement

Homeowners may struggle to find trustworthy tradespeople, compare service rates, purchase materials, and coordinate home-improvement work. Fundis may also lack a centralised platform to advertise their services and manage customer requests.

FundiShorp aims to bring these activities together in one digital marketplace.

## 1.3 Project Vision

To develop a trusted and accessible marketplace where homeowners can find skilled fundis, compare prices, purchase materials, and book services while enabling tradespeople to promote and grow their businesses.

## 1.4 Project Objectives

- Develop a React frontend connected to a Java Spring Boot backend.
- Design and implement a MySQL database.
- Support homeowner and fundi registration.
- Provide appropriate role-based access.
- Support fundi verification and storefront management.
- Enable product listing and pricing management.
- Support booking requests and booking management.
- Provide ratings and reviews where supported by the implementation.
- Use Trello and GitHub to manage and document project work.
- Test features and improve the product incrementally.

## 1.5 Project Scope

### In scope

- User registration and authentication.
- Homeowner and fundi accounts.
- Role-based access control.
- Fundi verification.
- Storefront and product management.
- Material and service pricing.
- Search and discovery of fundis.
- Booking management.
- Shopping cart and checkout features.
- Ratings and reviews.
- Database and API integration.
- Testing, documentation, and project demonstration.

The actual delivery status of each feature must be confirmed against the application and Trello board.

### Out of scope

Native mobile applications, international expansion, and advanced AI-based matching are not included in the initial scope unless formally approved as additional work.

## 1.6 Stakeholders

| Stakeholder | Interest or responsibility |
|---|---|
| Homeowners | Find fundis, compare prices, purchase materials, and book services |
| Fundis | Register, advertise services, manage listings, and handle bookings |
| Administrators | Manage access, review verification submissions, and oversee the platform |
| Development team | Plan, implement, test, and document features |
| Academic stakeholders | Review the project and its Agile evidence |

## 1.7 Agile Roles

| Role | Main responsibility |
|---|---|
| Product Owner | Clarifies requirements and prioritises the product backlog |
| Scrum Master | Supports the Scrum process and helps remove blockers |
| Development team | Builds and tests product increments |
| Stakeholders | Provide feedback and review outcomes |

Formal role assignments should be confirmed by the project team.

## 1.8 Project Constraints and Risks

- Limited academic project time.
- Dependencies between the database, backend, and frontend.
- Integration and testing complexity.
- Authentication and authorisation risks.
- Potential delays caused by unresolved defects or dependencies.
- The need to keep Trello and GitHub documentation consistent.

## 1.9 Success Criteria

The project will be evaluated against the following criteria:

- Required user roles and access rules work correctly.
- Database relationships and API operations behave as intended.
- Core registration and storefront workflows are testable.
- Product and pricing information is displayed accurately.
- Booking workflows follow the agreed requirements.
- User stories have clear acceptance criteria.
- Sprint tasks and progress are documented.
- Completed work is supported by appropriate evidence and testing.

---

# 2. User Stories and Tasks

User stories describe the functionality required by users or the development team. Tasks break each story into manageable pieces of work, while acceptance criteria define how the expected outcome can be checked.

The following stories retain the IDs and core content from the existing portfolio. Their acceptance criteria describe intended results and should not be interpreted as proof that every feature has been completed.

## Epic 1: Backend Architecture and Database

### US01 — Establish the Database Schema

**User story:** As a developer, I want a structured MySQL database so that application data and relationships can be managed consistently.

**Tasks**
- Design the entity relationship diagram.
- Define the required entities and relationships.
- Implement tables, constraints, and migrations where applicable.
- Add test data.
- Verify database operations.

**Acceptance criteria**
- Required entities and relationships are documented.
- Foreign-key relationships are valid.
- Required constraints are enforced.
- Database queries can be tested.

**Screenshot — Database Schema**

![FundiShorp Database Schema](screenshots/databaseschema.png)

### US02 — Build the Backend

**User story:** As a developer, I want a layered Java Spring Boot backend so that business logic and data access remain organised and maintainable.

**Tasks**
- Create domain or entity classes.
- Implement repositories.
- Develop service classes.
- Create REST controllers.
- Connect the backend to MySQL.
- Test API operations.

**Acceptance criteria**
- Controllers, services, and repositories have clear responsibilities.
- API operations return appropriate responses.
- Data is persisted and retrieved correctly.
- Errors are handled appropriately.

**Screenshot — Backend**

![FundiShorp Backend](screenshots/backend.png)

## Epic 2: Frontend Foundation

### US03 — Develop the React Frontend

**User story:** As a developer, I want a reusable React frontend so that users can navigate the application and interact with its features.

**Tasks**
- Set up the React project.
- Build reusable components.
- Configure routing.
- Connect the frontend to the backend API.
- Implement form validation.
- Test page navigation and responsiveness.

**Acceptance criteria**
- Main routes load correctly.
- Components use a consistent layout.
- API requests use the intended backend.
- Forms provide appropriate feedback.

**Screenshot — Frontend**

![FundiShorp Frontend](screenshots/frontend.png)

### US04 — Prepare Deployment

**User story:** As a developer, I want a repeatable deployment process so that the application can be tested and released reliably.

**Tasks**
- Document the deployment environment.
- Configure environment variables.
- Protect credentials and secrets.
- Prepare deployment scripts or a pipeline if required.
- Test deployment and document errors.

**Acceptance criteria**
- Deployment instructions are documented.
- Secrets are not committed to GitHub.
- The deployment result can be verified.

**Status:** Confirm actual deployment progress before marking this story complete.

## Epic 3: Accounts and Authentication

### US05 — Register as a Homeowner

**User story:** As a homeowner, I want to register for an account so that I can access the marketplace.

**Tasks**
- Build the registration form.
- Validate required fields.
- Connect the form to the API.
- Implement or connect authentication.
- Test valid and invalid submissions.

**Acceptance criteria**
- Valid registration details are accepted.
- Invalid details produce useful feedback.
- Credentials are handled securely.
- Successful registration follows the expected workflow.

**Screenshot — User Registration**

![FundiShorp User Registration](screenshots/register.png)

### US06 — Register as a Fundi

**User story:** As a fundi, I want to register for a trade account so that I can offer services through the marketplace.

**Tasks**
- Build the fundi registration form.
- Capture required trade information.
- Validate the submitted information.
- Connect the form to the backend.
- Test registration and error handling.

**Acceptance criteria**
- Required fundi information can be submitted.
- Invalid submissions are rejected.
- The account receives the appropriate role.
- Submitted information is handled securely.

**Screenshot — Fundi Registration**

![FundiShorp Fundi Registration](screenshots/fundireg.png)

### US07 — Manage User Roles

**User story:** As an administrator, I want role-based access control so that users can access only the functions permitted for their roles.

**Tasks**
- Define role permissions.
- Implement backend authorisation checks.
- Protect restricted frontend routes.
- Test authorised and unauthorised requests.

**Acceptance criteria**
- Roles have appropriate permissions.
- Protected backend operations enforce access rules.
- Unauthorised requests are rejected.

**Screenshot — User Roles**

![FundiShorp User Roles](screenshots/role.png)

## Epic 4: Verification and Storefronts

### US08 — Review Fundi Verification

**User story:** As an administrator, I want to review fundi verification submissions so that trade accounts can be assessed before approval.

**Tasks**
- Define the verification workflow.
- Provide access to submitted information.
- Implement approval and rejection operations where required.
- Test status updates and permissions.

**Acceptance criteria**
- Authorised administrators can review submissions.
- Approval decisions are recorded.
- Status changes are reflected correctly.

### US09 — Display Verification Status

**User story:** As a homeowner, I want to identify verified fundis so that I can make more informed choices.

**Tasks**
- Connect storefronts to verification status.
- Display the appropriate status indicator.
- Test approved and unapproved accounts.

**Acceptance criteria**
- Verification status reflects trusted application data.
- The interface does not incorrectly label unverified accounts as verified.

### US10 — Create and Manage a Fundi Storefront

**User story:** As a fundi, I want to manage my storefront so that customers can learn about my services and business.

**Tasks**
- Build the storefront interface.
- Display relevant business and trade information.
- Implement create, read, update, and delete operations where required.
- Test saving and retrieving storefront information.

**Acceptance criteria**
- Storefront information can be managed by authorised users.
- Saved information is displayed correctly.
- Unauthorised edits are rejected.

**Screenshot — Fundi Interface**

![FundiShorp Fundi Interface](screenshots/fundis.png)

## Epic 5: Product Listings and Pricing

### US11 — Add Products and Materials

**User story:** As a fundi, I want to add products and materials so that customers can browse available items.

**Tasks**
- Build the product form.
- Implement the listing API.
- Validate product details and prices.
- Support product images where required.
- Test saving and displaying listings.

**Acceptance criteria**
- Valid listings can be saved.
- Product details and prices display correctly.
- Invalid information is rejected.

### US12 — Edit and Remove Listings

**User story:** As a fundi, I want to update or remove my listings so that my storefront remains accurate.

**Tasks**
- Implement edit and delete operations.
- Add the relevant interface controls.
- Test updates and removal.
- Enforce ownership and permissions.

**Acceptance criteria**
- Authorised fundis can update their own listings.
- Removed listings are no longer offered as available.
- Unauthorised changes are rejected.

### US13 — View Product Details

**User story:** As a homeowner, I want to view product details so that I can make informed purchasing decisions.

**Tasks**
- Create a product details view.
- Display product information and images.
- Retrieve details from the backend.
- Test missing or invalid product references.

**Acceptance criteria**
- The correct product information is displayed.
- Prices and availability reflect saved data.
- Missing products are handled appropriately.

### US14 — Manage Booking and Service Pricing

**User story:** As a fundi, I want to manage service rates and booking information so that customers can understand the services I offer.

**Tasks**
- Develop the relevant pricing and booking interface.
- Connect the interface to the backend.
- Validate submitted values.
- Test saving and retrieving information.

**Acceptance criteria**
- Permitted information can be updated.
- Saved values display correctly.
- Invalid values are rejected.

**Screenshot — Booking Management**

![FundiShorp Booking Management](screenshots/booking.png)

### US15 — Display Job Pricing

**User story:** As a homeowner, I want to understand material and service costs so that I can estimate the cost of a job before proceeding.

**Tasks**
- Display material and service prices.
- Calculate totals where supported.
- Separate different cost components.
- Test calculations and displayed values.

**Acceptance criteria**
- Cost components are clearly identified.
- Totals are calculated correctly.
- Unconfirmed charges are not presented as final costs.

## Epic 6: Search, Cart and Customer Workflows

### US16 — Search for Fundis

**User story:** As a homeowner, I want to search for fundis by relevant criteria so that I can find a suitable tradesperson.

**Tasks**
- Create search and filter controls.
- Implement the search API.
- Display matching results.
- Test searches with different criteria.

**Acceptance criteria**
- Search results match the submitted criteria.
- Empty results are handled clearly.
- Verification status is displayed accurately where supported.

### Additional Backlog Stories

The following are additional product capabilities to track where they are included in the approved scope. Confirm their status and priority against Trello.

**US17 — Manage the Shopping Cart**

As a homeowner, I want to manage selected products so that I can review my intended purchases.

Tasks: Add items, update quantities, remove items, and calculate totals.

**US18 — Submit a Booking Request**

As a homeowner, I want to request a service booking so that I can arrange work with a fundi.

Tasks: Select a service, submit booking details, save the request, and display its status.

**US19 — Manage Reviews and Ratings**

As a homeowner, I want to review an eligible completed service so that I can share feedback about my experience.

Tasks: Submit a rating, validate review eligibility, save feedback, and display permitted reviews.

**US20 — Administrative Oversight**

As an administrator, I want to oversee users and relevant platform activity so that the marketplace can be managed appropriately.

Tasks: Review user information, enforce permissions, and test administrative actions.

---

# 3. Product Backlog

The Product Backlog is the prioritised list of product features, improvements, and requirements. It changes as the team receives feedback, discovers dependencies, and refines requirements.

The priorities below are **proposed starting priorities**, not confirmed Trello rankings. Confirm them with the Product Owner.

| ID | Product backlog item | Priority | Status |
|---|---|---|---|
| US01 | Database schema | High | Verify in Trello |
| US02 | Backend architecture and API | High | Verify in Trello |
| US03 | React frontend | High | Verify in Trello |
| US04 | Deployment preparation | Medium | Verify in Trello |
| US05 | Homeowner registration | High | Verify in Trello |
| US06 | Fundi registration | High | Verify in Trello |
| US07 | Role-based access | High | Verify in Trello |
| US08 | Fundi verification review | Medium | Verify in Trello |
| US09 | Verification status indicator | Medium | Verify in Trello |
| US10 | Fundi storefront management | High | Verify in Trello |
| US11 | Create product listings | High | Verify in Trello |
| US12 | Edit and remove listings | High | Verify in Trello |
| US13 | Product details | Medium | Verify in Trello |
| US14 | Booking and service pricing | High | Verify in Trello |
| US15 | Job pricing display | Medium | Verify in Trello |
| US16 | Search for fundis | High | Verify in Trello |
| US17 | Shopping cart | Medium | Verify in Trello |
| US18 | Booking requests | High | Verify in Trello |
| US19 | Reviews and ratings | Medium | Verify in Trello |
| US20 | Administrative oversight | Medium | Verify in Trello |

## Product Backlog Management

The team should:

- Refine stories before selecting them for a sprint.
- Prioritise work according to value, risk, and dependencies.
- Break large stories into smaller tasks.
- Define acceptance criteria for each story.
- Update priorities and statuses in Trello.
- Add new work when requirements change.

**Source of truth:** [FundiShorp Trello Board](https://trello.com/b/aviqvFPS/fundishorp)

---

# 4. Sprint Backlog

The Sprint Backlog contains the work selected for a sprint, the sprint goal, and the tasks required to deliver the selected increment.

The actual sprint assignments and completion statuses must be taken from the Trello board. The table below is a template for documenting the current sprint without inventing completion dates or results.

## 4.1 Sprint Planning

| Planning item | Details |
|---|---|
| Sprint number | Enter the actual sprint number |
| Sprint dates | Enter the actual start and end dates |
| Sprint goal | State the intended outcome |
| Selected stories | Record the Trello story IDs |
| Team capacity | Record available team capacity |
| Dependencies | Record tasks or features that must be completed first |

## 4.2 Sprint Tasks

| User story | Task | Assigned to | Status |
|---|---|---|---|
| US01 | Implement and verify database relationships | Confirm in Trello | Confirm in Trello |
| US02 | Implement backend API operations | Confirm in Trello | Confirm in Trello |
| US03 | Connect frontend components to the API | Confirm in Trello | Confirm in Trello |
| US05 | Implement and test registration | Confirm in Trello | Confirm in Trello |
| US07 | Verify role-based permissions | Confirm in Trello | Confirm in Trello |
| US10 | Implement storefront management | Confirm in Trello | Confirm in Trello |
| US11 | Implement product listing operations | Confirm in Trello | Confirm in Trello |
| US18 | Implement booking requests | Confirm in Trello | Confirm in Trello |

Only retain tasks that were actually selected for the sprint. Remove items that are not part of the current sprint and add the tasks shown on the actual board.

## 4.3 Sprint Execution

For each selected task, record:

- What work needs to be done.
- Who is responsible.
- Dependencies or blockers.
- Evidence of implementation.
- Testing results.
- Whether the acceptance criteria have been met.

## 4.4 Sprint Review

At the end of a sprint, document:

- Features demonstrated.
- Acceptance criteria met.
- Outstanding work.
- Stakeholder feedback.
- Items returned to or added to the Product Backlog.

## 4.5 Sprint Planning Evidence

![FundiShorp Trello Sprint Planning Board](screenshots/trello.png)

*The screenshot provides supporting evidence of project organisation. Update this section with the actual sprint goal, selected stories, and outcomes for the sprint being documented.*

---

# 5. Agile Logbook

The Agile Logbook records the work performed throughout development. It should show progress, decisions, challenges, solutions, and lessons learned.

Record actual events and dates. Do not mark work as completed unless there is supporting evidence.

## 5.1 Sprint Logbook

| Date / Sprint | Activities performed | Evidence or outcome | Challenges and lessons |
|---|---|---|---|
| Enter actual date | Record work completed | Link to commit, screenshot, or Trello card | Record actual findings |
| Enter actual date | Record work completed | Link to commit, screenshot, or Trello card | Record actual findings |
| Enter actual date | Record work completed | Link to commit, screenshot, or Trello card | Record actual findings |

Add rows as the project progresses.

## 5.2 Daily or Work-Session Log

For detailed work sessions, use the following format:

**Date:** Enter date  
**Sprint:** Enter sprint number  
**User story:** Enter story ID  
**Planned task:** Describe the intended work  
**Work completed:** Describe what was actually done  
**Testing performed:** Record tests and results  
**Blockers:** Record issues that prevented progress  
**Next action:** Identify the next task  
**Evidence:** Link to the relevant Trello card, GitHub commit, or screenshot

## 5.3 Retrospective and Continuous Improvement

At the end of each sprint, reflect on the following:

### What went well?
Record successful practices, completed work, and effective collaboration.

### What did not go well?
Identify delays, unclear requirements, technical problems, or missed expectations.

### What will be improved?
Specify practical actions, such as clarifying acceptance criteria, testing API endpoints earlier, or improving task allocation.

### Follow-up actions

| Improvement action | Responsible person | Target sprint | Status |
|---|---|---|---|
| Enter agreed action | Confirm owner | Enter sprint | Update from Trello |
| Enter agreed action | Confirm owner | Enter sprint | Update from Trello |

---

# 6. Supporting Evidence and References

## 6.1 Project Management Evidence

The Trello board supports the documentation of user stories, task breakdown, sprint planning, and progress tracking.

- [FundiShorp Trello Board](https://trello.com/b/aviqvFPS/fundishorp)
- [FundiShorp GitHub Repository](https://github.com/KabeloMoloko/FundiShorp-Portfolio)

## 6.2 Screenshot Index

The following screenshots are stored in the repository and referenced in the relevant user-story sections above.

| Screenshot | Purpose |
|---|---|
| `screenshots/databaseschema.png` | Database schema |
| `screenshots/backend.png` | Backend |
| `screenshots/frontend.png` | Frontend |
| `screenshots/register.png` | User registration |
| `screenshots/fundireg.png` | Fundi registration |
| `screenshots/role.png` | User roles |
| `screenshots/fundis.png` | Fundi interface |
| `screenshots/booking.png` | Booking management |
| `screenshots/trello.png` | Trello project board |

## 6.3 References

- [The Scrum Guide](https://scrumguides.org/scrum-guide.html) — Scrum roles, events, artefacts, and commitments.
- [GitHub Markdown Documentation](https://docs.github.com/en/get-started/writing-on-github) — README formatting and Markdown.
- [FundiShorp GitHub Repository](https://github.com/KabeloMoloko/FundiShorp-Portfolio) — Project documentation and screenshot evidence.
- [FundiShorp Trello Board](https://trello.com/b/aviqvFPS/fundishorp) — Product backlog and project task tracking.

---

**Portfolio note:** This document describes the intended functionality and Agile planning approach for FundiShorp. Actual implementation status, sprint results, and completed acceptance criteria should be verified against the application, GitHub commits, test results, and Trello board.
