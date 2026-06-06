# Security Rules

These rules enforce secure development practices across all projects.

## Code Integrity
- All code must be signed by a trusted developer key before merging to main.
- No hardcoded secrets in source files (use environment variables).

## Input Validation
- All user inputs must be sanitized and validated using OWASP standards.
- No direct execution of untrusted input strings.

## Authentication
- Use OAuth 2.0 for all external service integrations.
- Never store passwords in plain text; use bcrypt or scrypt.