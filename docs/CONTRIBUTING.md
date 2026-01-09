# Contributing Guide

## How to Contribute

### Reporting Issues
1. Search existing issues to avoid duplicates
2. Use issue templates
3. Provide detailed reproduction steps
4. Include system environment information

### Submitting Code
1. Fork the repository
2. Create feature branch
3. Follow code standards
4. Write test cases
5. Submit Pull Request

## Development Workflow

### Branch Strategy
- `main`: Stable version
- `develop`: Development version
- `feature/*`: Feature branches
- `hotfix/*`: Emergency fixes

### Commit Convention
```
type(scope): description

[optional body]

[optional footer]
```

Types:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation
- `style`: Formatting
- `refactor`: Refactoring
- `test`: Testing
- `chore`: Build

### Code Review
- All PRs require review
- Ensure tests pass
- Check code quality
- Verify functionality

## Development Standards

### TypeScript Standards
- Use strict mode
- Explicit type annotations
- Avoid any type
- Use interfaces for definitions

### Naming Conventions
- Classes: PascalCase
- Methods/Variables: camelCase
- Constants: UPPER_CASE
- Files: kebab-case

### Comment Standards
```typescript
/**
 * Character controller class
 * @description Manages character movement, animation and state
 */
class CharacterController {
    /**
     * Move character
     * @param direction Movement direction vector
     * @param speed Movement speed
     */
    move(direction: Vector3, speed: number): void {
        // Implementation logic
    }
}
```

## Testing Guidelines

### Unit Testing
- Use Jest framework
- Cover core functionality
- Mock external dependencies

### Integration Testing
- Test module interactions
- Verify API interfaces
- Check performance metrics

### Manual Testing
- Multi-browser testing
- Mobile device testing
- Performance stress testing
