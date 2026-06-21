Section 1
This Spring Boot application combines Spring MVC and REST controllers to support multiple user interfaces. The Admin and Doctor dashboards are rendered using Thymeleaf templates, while modules such as Appointments, PatientDashboard, and PatientRecord are exposed via REST APIs.

The backend follows a three-tier architecture:

Presentation Tier: Thymeleaf-based dashboards and REST API clients (mobile/web).

Application Tier: Spring Boot controllers, services, and business logic.

Data Tier: Dual databases — MySQL (structured data: patients, doctors, appointments, admin) and MongoDB (flexible prescriptions).

Controllers delegate requests to the Service Layer, which applies business rules and coordinates workflows. Services interact with Repositories that abstract database access. MySQL repositories use Spring Data JPA with @Entity classes, while MongoDB repositories use Spring Data MongoDB with @Document models.

This architecture ensures scalability, maintainability, and interoperability, supporting both server-rendered views and API-driven integrations.


Section 2

User Interface

Thymeleaf dashboards for Admin and Doctor.

REST API clients for appointments and patient modules.

Controller Layer

MVC Controllers return .html templates.

REST Controllers return JSON responses.

Service Layer

Applies business rules and validations.

Coordinates workflows (e.g., doctor availability checks).

Repository Layer

MySQL Repositories via Spring Data JPA.

MongoDB Repositories via Spring Data MongoDB.

Database Access

MySQL stores structured relational data.

MongoDB stores flexible prescription documents.

Model Binding

MySQL → JPA Entities (@Entity).

MongoDB → Document Models (@Document).

Application Models in Use

MVC: Models passed to Thymeleaf templates → HTML.

REST: Models/DTOs serialized → JSON responses.
