---
description: Rules for building professional, clean, and standard-compliant REST APIs in Java.
---

# Java Clean API Edicts

## 1. REST Standards
- **Nouns over Verbs**: Use `/users` not `/getUsers`.
- **Plurals**: Use `/products`, not `/product`.
- **HTTP Methods**:
  - `GET`: Idempotent, fetch data.
  - `POST`: Create resource.
  - `PUT`: Replace/Update entire resource.
  - `PATCH`: Partial update.
  - `DELETE`: Remove resource.
- **Status Codes**: 
  - `201 Created` for successful POST.
  - `204 No Content` for successful DELETE.
  - `400 Bad Request` for validation errors.
  - `404 Not Found` for missing resources.

## 2. Modern Java (21+)
- **Records**: Use `record` for DTOs and internal data carriers to ensure imutability.
- **Var**: Use `var` for local variables where the type is obvious.
- **Stream API**: Prefer functional streams over manual loops for data transformation.

## 3. Clean Code
- **No Nulls**: Use `Optional<T>` for return types that can be empty.
- **Validation**: Use Jakarta Bean Validation (`@NotNull`, `@Size`, etc.) on DTOs.
- **Global Exception Handling**: Use `@RestControllerAdvice` to map exceptions to standard RFC 7807 Error Responses.

## 4. Documentation
- **SpringDoc/OpenAPI**: Every API must expose a Swagger UI at `/swagger-ui.html`.
- **Meaningful Names**: Controller methods should reflect business actions, not just HTTP methods.
