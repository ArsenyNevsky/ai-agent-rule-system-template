# Testing Rules

Ensure all code is tested with high coverage and proper test structure.

## Test Coverage
- All new features must have 90%+ test coverage (measured via Istanbul).
- No code changes allowed into main without passing all tests.

## Test Design
- Write unit, integration, and end-to-end tests for all new components.
- Use `jest` or equivalent testing framework with proper mocking.

## Test Metadata
- All test files must include a `@test:smoke` or `@test:e2e` tag in the filename.
- Integration tests must be marked with a `@test:integration` tag and run in the CI pipeline.