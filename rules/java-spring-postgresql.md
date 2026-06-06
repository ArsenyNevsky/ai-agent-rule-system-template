# Java Spring Boot PostgreSQL Rule Set

Enforce best practices for Java, Spring Boot, and PostgreSQL-based applications.

## Code Structure
- Use package hierarchy: `com.example.project.domain`, `com.example.project.application`, `com.example.project.infrastructure`.
- All domain entities must be in `domain` package and annotated with `@Entity`.
- Services must use `@Service` annotation and follow interface-based design.

## Spring Boot Best Practices
- Inject dependencies using constructor injection, never field injection.
- Use `@Validated` for method-level validation and `@NotNull`, `@Size` annotations.
- All REST endpoints must use `@RestController` and return JSON via `ResponseEntity`.

## PostgreSQL Conventions
- Use snake_case for all table and column names (e.g., `user_profile`, `created_at`).
- Primary keys must be named `id` and use auto-incrementing sequences.
- Always define indexes on foreign keys and frequently queried columns.

## Testing Standards
- Write unit tests for all services using `@MockBean` and `@SpringBootTest`.
- Integration tests must test database interactions using H2 in-memory DB for speed.
- Use `@Transactional` on integration tests to ensure rollback after each test.

## Security
- All endpoints must be secured with Spring Security using JWT authentication.
- Never expose sensitive fields in API responses; use `@JsonIgnore` or DTOs for serialization.

## Architectural Principles
- Single responsibility principle: each class should have one reason to change.
- Dependency inversion: high-level modules must not depend on low-level ones; use interfaces throughout.
- Avoid `@Autowired` in constructors—use constructor injection only.