
# FundiShorp – Agile Project Portfolio

![FundiShorp Website](screenshots/web.png)


## Project Overview

FundiShorp is a proposed online platform designed to connect homeowners with fundis (skilled tradespeople) who provide home improvement, maintenance, repair and construction services. The platform also aims to allow fundis to advertise their services and building materials to potential customers.

This portfolio documents my work on the FundiShorp project using Agile project management principles. It presents the project charter, user stories, product backlog, sprint planning and supporting evidence of the work completed during the project.

The project is being developed incrementally, with tasks and requirements organised to support planning, implementation, testing and continuous improvement.

## 1. Agile Project Charter

### 1.1 Project Purpose

The purpose of FundiShorp is to make it easier for homeowners to find suitable tradespeople and access services or materials needed for home improvement projects. The platform is intended to provide a central place where customers can explore available fundis and where service providers can present their offerings.

### 1.2 Problem Statement

Finding reliable tradespeople and comparing their services can be difficult when information is spread across different sources. Customers may also struggle to identify service providers who have been verified.

FundiShorp aims to address this problem by providing an online platform where users can find fundis, view available services and materials, and access relevant information before making decisions.

### 1.3 Project Objectives

The main objectives of the project are to:

- Develop a user-friendly frontend for the platform.
- Create a backend to process application requests and manage data.
- Design and connect a MySQL database.
- Support homeowner and fundi registration.
- Apply role-based access according to user roles.
- Allow fundis to manage their service or product listings.
- Provide functionality for searching and viewing available fundis.
- Organise project requirements and development tasks using Agile methods.
- Document project progress and provide supporting evidence.

### 1.4 Project Scope

**Included in the project:**

- User registration and login.
- Fundi registration and profile management.
- Role-based access control.
- Fundi verification-related functionality.
- Storefront and product listing management.
- Viewing product and service information.
- Searching for fundis.
- Database and backend development.
- Agile planning and project documentation.

**Outside the initial scope:**

- A fully operational payment gateway.
- A production-scale mobile application.
- Advanced analytics and automated recommendations.

These items may be considered for future development if time and resources allow.

### 1.5 Technologies and Tools

| Technology or tool | Purpose |
|---|---|
| React | Developing the user interface |
| Java Spring Boot | Developing backend services and API endpoints |
| MySQL | Storing and managing application data |
| Git and GitHub | Version control and project hosting |
| Trello | Managing the product backlog and sprint tasks |
| GitHub Pages | Publishing the project portfolio |

### 1.6 Agile Approach

I am using an Agile approach to organise the project into manageable tasks and prioritise the development of important features. User stories describe the needs of different users, while tasks break the work into smaller activities.

Trello is used to organise the backlog and track project activities. The project can be reviewed and adjusted as development progresses, allowing requirements and priorities to be refined when necessary.

### 1.7 Stakeholders

The main stakeholders are:

- **Homeowners:** People who need home improvement services or building materials.
- **Fundis:** Tradespeople who want to advertise their skills, services or products.
- **Administrator:** A user responsible for managing platform activities and verification-related processes.
- **Developer:** The student responsible for planning, developing, testing and documenting the project.

### 1.8 Expected Outcomes

The expected outcome is a functional web application prototype that demonstrates the main requirements of the FundiShorp platform. The project portfolio also provides evidence of Agile planning, technical development and project documentation.

---

## 2. User Stories and Tasks

The following user stories describe the main requirements identified for FundiShorp. Each story represents a feature or capability from the perspective of a user or the development team.

The screenshots provide supporting evidence of selected development activities. The presence of a screenshot does not necessarily mean that the feature has been fully tested or completed.

### US01 – Establish the Database Schema

**User story:** As a developer, I want to create a database schema so that application data can be stored in a structured way.

**Tasks:**
- Identify the main entities and their attributes.
- Define primary and foreign keys.
- Establish relationships between database tables.
- Create the schema in MySQL.
- Check the relationships and constraints.

**Acceptance criteria:**
- The required tables are created.
- Primary keys and relationships are defined where required.
- The schema supports the planned application features.

![FundiShorp Database Schema](screenshots/databaseschema.png)

### US02 – Develop the Backend

**User story:** As a developer, I want to develop backend services so that the frontend can communicate with the database through an API.

**Tasks:**
- Set up the Spring Boot project.
- Organise the backend into appropriate layers.
- Create the required models, repositories and services.
- Develop REST API endpoints.
- Configure the database connection.
- Test API requests and responses.

**Acceptance criteria:**
- The backend starts successfully.
- API endpoints process supported requests.
- Database operations work for the implemented features.
- Errors are handled appropriately.

![FundiShorp Backend](screenshots/backend.png)

### US03 – Develop the Frontend

**User story:** As a user, I want a clear and accessible interface so that I can navigate the platform and use its features.

**Tasks:**
- Set up the React application.
- Create reusable interface components.
- Develop the main pages and navigation.
- Connect frontend components to available API endpoints.
- Test page layout and navigation.

**Acceptance criteria:**
- The main pages display correctly.
- Users can navigate between available sections.
- Implemented frontend features communicate with the backend where required.

![FundiShorp Frontend](screenshots/frontend.png)

### US04 – Prepare for Deployment

**User story:** As a developer, I want to prepare the application for deployment so that it can be accessed and demonstrated online.

**Tasks:**
- Review application configuration.
- Identify hosting requirements for the frontend and backend.
- Configure environment-specific settings.
- Test the deployment process.
- Document any remaining deployment limitations.

**Acceptance criteria:**
- Deployment requirements are documented.
- The frontend can be prepared for hosting.
- Backend and database hosting requirements are identified.

### US05 – Register and Log In as a Homeowner

**User story:** As a homeowner, I want to register and log in so that I can access the platform using my account.

**Tasks:**
- Create the registration interface.
- Create the login interface.
- Validate submitted information.
- Connect the forms to the relevant backend endpoints.
- Test registration and login scenarios.

**Acceptance criteria:**
- Users can submit registration details.
- Required fields are validated.
- Login requests are processed by the backend.
- Feedback is provided when a request succeeds or fails.

![FundiShorp User Registration](screenshots/register.png)

### US06 – Register as a Fundi

**User story:** As a fundi, I want to register my details so that I can offer my services through the platform.

**Tasks:**
- Create the fundi registration form.
- Capture the required profile information.
- Include relevant verification information where required.
- Connect the form to the backend.
- Test form validation and data submission.

**Acceptance criteria:**
- Fundis can submit their registration information.
- Required information is validated.
- Submitted information is handled by the backend.

![FundiShorp Fundi Registration](screenshots/fundireg.png)

### US07 – Apply Role-Based Access

**User story:** As a platform user, I want access to features appropriate to my role so that different types of users have the correct permissions.

**Tasks:**
- Define the required user roles.
- Associate roles with user accounts.
- Apply access rules to relevant features.
- Test access for different roles.

**Acceptance criteria:**
- User roles are identified.
- Access to protected features is controlled according to the implemented rules.
- Users cannot access restricted functions without the required permissions.

![FundiShorp User Roles](screenshots/role.png)

### US08 – Review Fundi Verification Documents

**User story:** As an administrator, I want to review fundi verification information so that I can assess whether a fundi meets the platform's verification requirements.

**Tasks:**
- Identify the required verification information.
- Provide a way to review submitted details.
- Record verification decisions where implemented.
- Test the verification workflow.

**Acceptance criteria:**
- Relevant verification information can be reviewed.
- Verification decisions can be recorded if the workflow is implemented.
- The status is available to the relevant parts of the application.
![FundiShorp Verification Evidence](screenshots/veri.png)

### US09 – Display a Verified Badge

**User story:** As a homeowner, I want to identify verified fundis so that I can make a more informed decision when selecting a service provider.

**Tasks:**
- Define the verification status used by the application.
- Connect the status to the fundi profile.
- Display the badge when the required conditions are met.
- Test verified and unverified profiles.

**Acceptance criteria:**
- Verification status is represented consistently.
- A verified badge is displayed only when the required verification condition is satisfied.

### US10 – Create a Storefront

**User story:** As a fundi, I want to create a storefront so that customers can view information about my services or products.

**Tasks:**
- Design the storefront interface.
- Capture storefront information.
- Connect storefront data to the backend.
- Display the information on the relevant page.

**Acceptance criteria:**
- A fundi can provide storefront information where the feature is implemented.
- Storefront information is displayed appropriately.
- The interface supports the planned service or product listings.

![FundiShorp Fundi Interface](screenshots/fundis.png)

### US11 – Add Products and Building Materials

**User story:** As a fundi, I want to add products or building materials so that customers can view what I offer.

**Tasks:**
- Create a product listing form.
- Capture product details and prices.
- Validate submitted information.
- Save listing information through the backend.
- Display available listings.

**Acceptance criteria:**
- Required product information is validated.
- Product details can be saved when the feature is connected.
- Saved listings can be retrieved for display.

### US12 – Edit and Remove Listings

**User story:** As a fundi, I want to edit or remove my listings so that I can keep my information up to date.

**Tasks:**
- Implement listing retrieval.
- Add an edit function.
- Add a delete function.
- Apply appropriate access restrictions.
- Test changes and removal.

**Acceptance criteria:**
- Authorised users can update their listings.
- Authorised users can remove their listings.
- Changes are reflected in the stored data.

### US13 – View Product Details

**User story:** As a homeowner, I want to view product details so that I can understand what is being offered before making a decision.

**Tasks:**
- Create a product details page or component.
- Display available descriptions and prices.
- Retrieve listing information from the backend.
- Test the display of available product information.

**Acceptance criteria:**
- Relevant product details are displayed.
- The correct listing information is shown.
- Missing or unavailable information is handled appropriately.

### US14 – Set Labour and Callout Rates

**User story:** As a fundi, I want to provide my labour and callout rates so that customers can understand the costs associated with my services.

**Tasks:**
- Define the required rate fields.
- Provide a form for entering rates.
- Validate the rate values.
- Save and retrieve the information.
- Display rates where applicable.

**Acceptance criteria:**
- Rate information is validated.
- Saved rates can be retrieved when the feature is implemented.
- Customers can view the available pricing information.

![FundiShorp Booking and Pricing Evidence](screenshots/booking.png)

### US15 – Display Combined Job Pricing

**User story:** As a homeowner, I want to view the available job pricing information so that I can better understand the potential cost of a service.

**Tasks:**
- Identify the pricing information required.
- Define how labour and callout rates should be presented.
- Display the available pricing information.
- Test the displayed values.

**Acceptance criteria:**
- Available pricing information is presented clearly.
- The displayed amounts correspond to the relevant service or fundi.
- Any estimate is clearly distinguished from a confirmed final price.

### US16 – Search for Verified Fundis

**User story:** As a homeowner, I want to search for fundis so that I can find service providers who match my needs.

**Tasks:**
- Create the search interface.
- Retrieve relevant fundi information.
- Provide filtering or search criteria where supported.
- Display matching results.
- Test search results and empty searches.

**Acceptance criteria:**
- Users can search using the supported criteria.
- Matching fundis are displayed.
- Empty results are handled appropriately.
- Verification information is displayed accurately where available.
![FundiShorp Search](screenshots/search.png)


### US17 – Submit a Service Booking Request

**User story:** As a homeowner, I want to submit a booking request so that I can request a service from a fundi.

**Acceptance criteria:**
- A homeowner can submit the required booking details.
- The request is stored if the booking functionality is implemented.
- The relevant status can be viewed by authorised users.

### US18 – Review a Fundi

**User story:** As a homeowner, I want to submit a review after receiving a service so that I can share feedback about my experience.

**Acceptance criteria:**
- A review can be submitted through the implemented interface.
- Review data is validated and stored.
- Reviews are associated with the relevant fundi.
![FundiShorp Reviews](screenshots/review.png)

### US19 – Manage Booking Requests

**User story:** As a fundi, I want to view and manage booking requests so that I can respond to potential customers.

**Acceptance criteria:**
- Relevant booking requests can be viewed.
- A fundi can update a request's status where the feature is implemented.
- Changes are reflected in the stored information.

### US20 – Administer Platform Information

**User story:** As an administrator, I want to manage relevant platform information so that the application can be maintained appropriately.

**Acceptance criteria:**
- Administrative functions are restricted to authorised users.
- Supported management actions are recorded or reflected in the application.
- Invalid actions are handled appropriately.
![FundiShorp Booking Management](screenshots/managebooking.png)

---

## 3. Product Backlog

The product backlog contains the features and improvements identified for the FundiShorp project. Items are organised according to their importance to the project's objectives.

The priorities below are proposed priorities for documentation purposes. The Trello board should be treated as the working source for the latest task status and sprint allocation.

| ID | Backlog item | Priority | Status |
|---|---|---|---|
| US01 | Establish database schema | High | Verify in Trello |
| US02 | Develop backend services | High | Verify in Trello |
| US03 | Develop React frontend | High | Verify in Trello |
| US04 | Prepare for deployment | Medium | Verify in Trello |
| US05 | Homeowner registration and login | High | Verify in Trello |
| US06 | Fundi registration | High | Verify in Trello |
| US07 | Role-based access | High | Verify in Trello |
| US08 | Fundi verification review | Medium | Verify in Trello |
| US09 | Verified fundi badge | Medium | Verify in Trello |
| US10 | Create a storefront | High | Verify in Trello |
| US11 | Add product and material listings | High | Verify in Trello |
| US12 | Edit and remove listings | Medium | Verify in Trello |
| US13 | View product details | Medium | Verify in Trello |
| US14 | Set labour and callout rates | Medium | Verify in Trello |
| US15 | Display job pricing | Medium | Verify in Trello |
| US16 | Search for verified fundis | High | Verify in Trello |
| US17 | Submit booking requests | Future | Proposed |
| US18 | Submit reviews | Future | Proposed |
| US19 | Manage booking requests | Future | Proposed |
| US20 | Administer platform information | Future | Proposed |

The backlog can be updated as requirements change, new issues are identified or tasks are completed. The priority and status of each item should be reviewed against the current Trello board.

**Trello project board:** [View the FundiShorp board](https://trello.com/b/aviqvFPS/fundishorp)

---


## 4. Sprint Backlog

The sprint backlog contains the user stories and development tasks selected for implementation during a sprint. For FundiShorp, I used an incremental approach to organise the work into database development, application development, feature integration, testing and documentation.

The tasks were broken down into smaller activities so that I could track progress, identify technical problems and determine what needed to be completed next. Trello was used to organise the backlog and monitor the project tasks.

### 4.1 Sprint 1 – Database and Project Setup

**Sprint goal:** Establish the technical foundation required for the FundiShorp application.

| User story | Development task | Expected result | Status |
|---|---|---|---|
| US01 – Database schema | Identify the main entities and relationships. | Database structure supports the planned features. | Verify against MySQL |
| US01 – Database schema | Create the required tables, keys and relationships in MySQL. | Tables and relationships are available for development. | Verify against MySQL |
| US02 – Backend | Configure the Spring Boot project and database connection. | Backend is configured to communicate with MySQL. | Test connection |
| US03 – Frontend | Review the React project structure and main pages. | Frontend structure is ready for feature integration. | Verify in application |

**Sprint review:** The database, backend and frontend form the foundation of the project. The next step is to test the database connection and confirm that the application components can communicate correctly.

### 4.2 Sprint 2 – User Registration and Access Control

**Sprint goal:** Develop the account-related functionality needed for homeowners and fundis.

| User story | Development task | Expected result | Status |
|---|---|---|---|
| US05 – Homeowner registration | Develop and validate the registration form. | Users can submit the required registration details. | Test in application |
| US05 – Login | Connect login requests to the relevant backend endpoint. | Login requests are processed by the backend. | Verify API and authentication |
| US06 – Fundi registration | Capture the required fundi profile information. | Fundi registration details can be submitted. | Test in application |
| US07 – User roles | Define roles and the relevant access restrictions. | Access rules are applied to protected features. | Verify permissions |
| US08 – Verification | Identify and display the information required for fundi verification. | Verification information can be reviewed where implemented. | Verify workflow |

**Sprint review:** Registration and access control are important because the platform has different user types. Testing should include valid and invalid registration details and checks that users cannot access restricted functions without the required permissions.

### 4.3 Sprint 3 – Fundi Profiles and Product Listings

**Sprint goal:** Develop the functionality that allows fundis to present their services and products.

| User story | Development task | Expected result | Status |
|---|---|---|---|
| US09 – Verified badge | Display the fundi verification status where available. | Verification status is presented accurately. | Verify status logic |
| US10 – Storefront | Develop the fundi storefront interface. | Fundi information can be displayed. | Verify in application |
| US11 – Product listings | Create the form for product and building material details. | Listing details can be submitted. | Test API integration |
| US12 – Listing management | Implement update and delete operations for listings. | Authorised users can manage their listings. | Test CRUD operations |
| US13 – Product details | Display the details of a selected listing. | Customers can view available product information. | Verify displayed data |
| US14 – Pricing | Capture and display labour and callout rates. | Available service pricing is presented clearly. | Verify calculations and display |

**Sprint review:** The storefront and listing features help fundis present their offerings. The main focus is to confirm that listing information is validated, saved correctly and displayed consistently.

### 4.4 Sprint 4 – Booking, Reviews and API Integration

**Sprint goal:** Integrate customer-facing features with the backend and database, and test the relevant operations.

| User story | Development task | Expected result | Status |
|---|---|---|---|
| US16 – Fundi search | Implement or review the search interface and available criteria. | Users can search for matching fundis where supported. | Test search results |
| Booking management | Connect the booking interface to the relevant API endpoints. | Booking information can be retrieved and managed where implemented. | Verify API and database |
| Reviews and ratings | Develop the review submission functionality. | Review information can be submitted and validated. | Test submission |
| Reviews and ratings | Implement or test review retrieval, editing and deletion where supported. | Review records can be managed through the API. | Test CRUD operations |
| Database integration | Check whether submitted records are saved in MySQL. | Stored records match successful requests. | Verify with SQL queries |
| Error handling | Test invalid input and unsuccessful requests. | The application provides appropriate error feedback. | Test and record issues |

**Sprint review:** This sprint focuses on connecting the user interface to the backend rather than relying on interface appearance alone. Postman can be used to test API requests, while MySQL queries can confirm whether the relevant data has been stored or updated.

### 4.5 Sprint 5 – Testing, Corrections and Portfolio Preparation

**Sprint goal:** Verify the implemented functionality, resolve outstanding issues and prepare the project portfolio for assessment.

| Task | Expected result | Status |
|---|---|---|
| Test registration and login | Confirm expected responses for valid and invalid inputs. | Outstanding verification |
| Test database operations | Check records created, retrieved, updated or deleted through the API. | Outstanding verification |
| Test reviews and ratings | Confirm review persistence and supported management operations. | Outstanding verification |
| Test booking management | Confirm booking data and status changes where implemented. | Outstanding verification |
| Check frontend and backend integration | Confirm that requests and responses use the expected formats. | Outstanding verification |
| Correct identified defects | Resolve and retest issues found during testing. | As issues are identified |
| Update README and Agile logbook | Document project activities, user stories and supporting evidence. | Update before submission |
| Check screenshots on GitHub Pages | Confirm that all referenced images display correctly. | Final portfolio check |

**Sprint review:** The purpose of this sprint is to assess the application against its requirements, identify remaining work and ensure that the portfolio accurately represents the state of the project.

### 4.6 Sprint Tracking and Evidence

The following Trello board is used to organise project tasks and review their current status.

[FundiShorp Trello Board](https://trello.com/b/aviqvFPS/fundishorp)

![FundiShorp Trello Board](screenshots/trello.png)

The screenshots in the `screenshots` folder provide supporting evidence of selected application interfaces and development activities. They should be considered alongside functional testing results when determining whether a feature is complete.

---

## 5. Agile Logbook

This logbook records my progress while planning, developing and documenting the FundiShorp project. I used it to reflect on the work completed, challenges encountered and tasks that still needed attention. I also used Trello to organise the project requirements and development activities.

The project was developed incrementally. Some activities focused on planning and implementation, while others involved troubleshooting, testing and improving the project documentation.

### 5.1 Development Activity Log

| Date | Activity and Work Performed | Outcome and Evidence | Challenges and Next Steps |
|---|---|---|---|
| 9 October 2026 | Reviewed the existing FundiShorp application to identify incomplete features and areas that needed improvement. I also considered how the database should connect to the application. | Identified database integration and application functionality as important areas for further development. | Review the database structure, confirm the required relationships and plan the connection between the frontend, backend and database. |
| 22 October 2026 | Worked on bringing the application components together and reviewing the React frontend and backend project files. | Continued the integration work and identified areas that required testing to confirm that the components communicated correctly. | Test the API endpoints and verify that information submitted through the frontend is processed correctly by the backend. |
| 23 October 2026 | Worked on event-related API operations and checked how submitted information could be stored in MySQL. Used Postman to test requests and investigate connection and request-format errors. | Worked through API testing issues and continued checking the relationship between the API responses and database records. | Continue testing valid and invalid requests, confirm that records are saved correctly, and check the results directly in MySQL. |
| 24 October 2026 | Continued development of the Reviews and Ratings functionality. Worked on the API operations for creating, retrieving, editing and deleting review records, and on connecting the React Reviews and Reports page to the API. | Established the main review-management tasks and continued the integration work needed to persist reviews in MySQL. | Verify each CRUD operation, confirm that reviews remain in the database after refreshing the page, and test error handling. |
| 27 October 2026 | Updated the FundiShorp project portfolio and organised screenshots showing selected parts of the website, frontend, backend, database schema, registration, roles, booking management, reviews and verification interfaces. | Added supporting screenshots to the repository and improved the structure of the project documentation. | Check that all image paths work on GitHub Pages, ensure that the screenshots match the relevant user stories, and review the final portfolio before submission. |

### 5.2 Sprint Reflection

#### Reflection on Planning and Development

During this project, I learned that developing a web application involves more than creating pages that look correct. The frontend, backend and database must work together for information to be processed and stored reliably.

One of the main areas requiring attention was API integration. Testing requests helped me identify problems with request formats, connections and the way the application communicates with the backend. This showed me the importance of testing individual components before relying on the complete application.

I also learned that features such as reviews and ratings require both frontend and backend work. A review form alone is not sufficient; the application must also validate the submitted information, process the request and store the data correctly.

#### What Went Well

- Breaking the application into smaller features made the work easier to organise.
- Using Postman provided a way to test API requests separately from the React interface.
- Checking MySQL records helped me investigate whether data was being stored.
- Organising screenshots made it easier to present the technical work in my portfolio.
- Documenting user stories helped connect the development activities to the needs of homeowners, fundis and administrators.

#### Challenges Encountered

- Connecting the frontend, backend and database required careful checking of endpoints and request formats.
- API testing involved troubleshooting errors before the expected results could be confirmed.
- Features needed to be checked at more than one level, including the user interface, API response and database records.
- Keeping the portfolio documentation consistent with the actual implementation required additional attention.

#### Improvements for the Next Sprint

- Test each API endpoint using valid, invalid and incomplete input.
- Confirm that create, read, update and delete operations work as expected.
- Check database records after submitting or updating information through the application.
- Record testing results and outstanding issues in Trello.
- Keep screenshots and documentation up to date as features change.
- Prioritise fixing integration problems before adding more functionality.

### 5.3 Lessons Learned

**1. Database design and integration**

The database must support the application's requirements and use appropriate relationships and constraints. Checking stored records is an important part of confirming that database operations work as expected.

**2. API testing**

Testing endpoints separately helps identify whether a problem comes from the request, backend logic or database connection. Tools such as Postman are useful for this purpose.

**3. Frontend and backend integration**

The React interface must send information in the format expected by the backend and handle the responses returned by the API. Integration should be tested rather than assumed to work.

**4. Testing and verification**

A feature should not be marked complete simply because its interface is visible. Its main operations should be tested, and the results should be checked against the acceptance criteria.

**5. Agile planning and documentation**

Maintaining a backlog, reviewing progress and recording outstanding tasks helps me understand what has been completed and what still needs work. Updating the portfolio alongside development also makes the final submission easier to prepare.

### 5.4 Current Project Position

At the time of preparing this portfolio, the project includes documented requirements, selected interface and development screenshots, and ongoing work involving application integration and review functionality.

The next priority is to verify the implemented features through functional testing, confirm that the relevant database operations work correctly, resolve outstanding issues and update the backlog to reflect the actual status of each task.

I will use the results of these checks to determine which features are complete, which require further work and which should be considered for future development.

---

## 6. Supporting Evidence and References

This section provides links and screenshots that support the project documentation.

### 6.1 Project Links

- [FundiShorp GitHub Repository](https://github.com/KabeloMoloko/FundiShorp-Portfolio)
- [FundiShorp GitHub Pages Portfolio](https://kabelomoloko.github.io/FundiShorp-Portfolio/)
- [FundiShorp Trello Board](https://trello.com/b/aviqvFPS/fundishorp)


---

## Conclusion

Working on FundiShorp has allowed me to apply Agile project management concepts while developing a web application. The project combines requirements planning, user stories, backlog management, frontend development, backend development and database design.

This portfolio brings the main project documentation and selected development evidence together in one place. As development continues, I will update the backlog, record progress in the Agile logbook, test implemented features and revise the documentation to reflect the actual state of the application.

