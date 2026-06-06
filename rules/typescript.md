# TypeScript Rules

Enforce consistent and type-safe coding practices for TypeScript projects.

## Type Safety
- All function parameters must have explicit types (never `any`).
- Use interfaces or type aliases for all complex object shapes.
- Never use `@ts-ignore` without a documented justification in the code comment.

## Function Design
- Functions must not exceed 30 lines of code.
- Use `const` over `let` for all variable declarations unless mutation is required.

## Error Handling
- All async functions must handle errors using `try/catch` or proper error callbacks.
- Never throw raw strings; always use structured error objects.