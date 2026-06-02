---
description: Architectural guidelines for Spring Boot projects focusing on Clean Architecture.
---

# Spring Boot Architecture Edicts

## 1. Layered Separation (Clean Arch)
- **Web/Controller Layer**: Only handles HTTP requests, validation, and mapping DTOs. No business logic.
- **Service/Domain Layer**: The heart of the application. Contains business rules. Orchestrates calls to repositories.
- **Infrastructure/Persistence Layer**: Entity definitions and Spring Data Repositories.

## 2. Dependency Injection
- **Constructor Injection**: ALWAYS use constructor-based injection. Avoid `@Autowired` on fields.
- **Interface Segregation**: Inject interfaces where possible to allow for easier mocking in tests.

## 3. Data Transfer
- **DTOs vs Entities**: Never expose JPA Entities directly to the Controller. Always map to/from DTOs using MapStruct or manual mappers.

## 4. Configuration
- **Profiles**: Use `application-dev.yml` for local dev and `application-prod.yml` for production.
- **Externalized Config**: Use `@ConfigurationProperties` for grouping related settings.

## 5. Security
- **Spring Security**: Use a stateless approach (JWT) for REST APIs.
- **Method Security**: Use `@PreAuthorize` to secure business logic at the service level.
