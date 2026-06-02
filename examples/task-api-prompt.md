# Example Prompt: Library Management System

This is an example of a high-signal prompt that leverages the full power of the multi-agent system.

## The Prompt

```text
Maestro, I need to implement a "Library Management System" using Spring Boot 3.x and PostgreSQL.

Requirements:
1. Domain: Books (ISBN, Title, Author, Year), Members (Name, Email, JoinDate), and Loans.
2. Rules: A member can have max 3 books at a time. Loans are for 14 days.
3. Architecture: Follow the project's 'spring-boot-architecture.md' (Service-Repository pattern).
4. DevOps: I need a Dockerfile and docker-compose for the app and DB.
5. Testing: Ensure the BookService has unit tests.

Please run the full lifecycle: Plan -> Review -> Implementation -> Security Audit.
```

## Why this works
- **Explicit Domain**: Provides clear entities and attributes.
- **Business Logic**: Defines constraints for the Coder and Reviewer to validate.
- **Rule Reference**: Explicitly points to the framework's internal rules.
- **Multi-Persona Request**: Commands the Maestro to use Architect, Coder, DevOps, and Reviewer.
