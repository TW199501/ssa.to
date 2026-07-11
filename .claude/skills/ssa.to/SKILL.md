```markdown
# ssa.to Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill documents the development patterns and conventions used in the `ssa.to` repository, a TypeScript codebase built with React. It covers file organization, code style, commit patterns, and testing approaches, providing clear examples and suggested commands for common workflows.

## Coding Conventions

### File Naming
- Use **camelCase** for all file names.
  - Example: `userProfile.tsx`, `apiClient.ts`

### Import Style
- Prefer **relative imports** for referencing modules within the project.
  - Example:
    ```typescript
    import { fetchData } from './apiClient';
    ```

### Export Style
- Use **named exports** for all modules.
  - Example:
    ```typescript
    // In userProfile.tsx
    export function UserProfile() { ... }
    ```

### Commit Patterns
- Commit messages are **freeform** (no enforced type or scope).
- Some commits use prefixes, but not consistently.
- Average commit message length is **196 characters**.
  - Example:
    ```
    Fix: resolve issue with user authentication flow when token expires during session
    ```

## Workflows

_No automated workflows detected in repository._

## Testing Patterns

- **Test File Pattern:** All test files follow the `*.test.*` naming convention.
  - Example: `userProfile.test.tsx`
- **Testing Framework:** Not explicitly detected; check project dependencies for details.
- **Test Example:**
  ```typescript
  // userProfile.test.tsx
  import { render } from '@testing-library/react';
  import { UserProfile } from './userProfile';

  test('renders user profile', () => {
    render(<UserProfile />);
    // assertions here
  });
  ```

## Commands
| Command | Purpose |
|---------|---------|
| /test   | Run all tests in files matching `*.test.*` |
| /lint   | Lint the codebase according to project standards |
| /build  | Build the project for production deployment |
| /start  | Start the development server |
```
