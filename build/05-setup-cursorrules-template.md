# .cursorrules Template for Rapid MVP Development

Use this template to create a `.cursorrules` file in your project root. This file provides strong rules and guidelines for Cursor to follow when building your MVP.

```markdown
# Rapid MVP Development Rules

## Core Principles

- **MVP First**: Focus on the minimum viable features that demonstrate core value. Avoid over-engineering.
- **Quality Over Speed**: Write clean, maintainable code even in rapid development. Technical debt should be intentional and documented.
- **Type Safety**: Use TypeScript strictly. Avoid `any` types. Use proper interfaces and types.
- **Component Reusability**: Create reusable components and utilities. Don't duplicate code.

## Code Quality Standards

### TypeScript
- Use strict TypeScript configuration
- Define explicit types for all function parameters and return values
- Use interfaces for object shapes, types for unions/primitives
- Prefer type inference where it improves readability, but be explicit for public APIs
- No `any` types unless absolutely necessary (and document why)

### React Best Practices
- Use functional components with hooks
- Keep components small and focused (single responsibility)
- Extract complex logic into custom hooks
- Use proper dependency arrays in useEffect, useMemo, useCallback
- Memoize expensive computations and components when appropriate
- Handle loading and error states explicitly

### Code Organization
- Follow a clear folder structure:
  - `src/components/` - Reusable UI components
  - `src/pages/` or `src/routes/` - Page-level components
  - `src/hooks/` - Custom React hooks
  - `src/utils/` - Utility functions
  - `src/store/` - State management (Zustand)
  - `src/types/` - TypeScript type definitions
  - `src/services/` - API calls and external services
- One component per file
- Use index files for clean imports
- Keep related files close together

### Error Handling
- Always handle errors explicitly
- Use try-catch for async operations
- Provide meaningful error messages to users
- Log errors appropriately (to console in dev, to LogRocket in prod)
- Never silently fail

### Testing Considerations
- Write testable code (pure functions where possible)
- Keep business logic separate from UI components
- Make components easy to test (accept props, avoid hidden dependencies)

## Technology Stack Conventions

### React 19 + TypeScript
- Use React 19 features appropriately
- Leverage TypeScript for type safety
- Use React Server Components where applicable (if using Next.js)

### State Management (Zustand)
- Keep stores focused and scoped
- Use TypeScript for store state shapes
- Avoid deeply nested state
- Use selectors for derived state

### Styling (Tailwind CSS)
- Use Tailwind utility classes primarily
- Create reusable component classes when needed
- Follow mobile-first responsive design
- Use design tokens/theme values consistently
- Ensure WCAG AA contrast ratios

### UI Components (Radix UI)
- Use Radix UI primitives for accessibility
- Don't override accessibility features
- Customize styling through Tailwind, not by breaking Radix APIs
- Follow Radix patterns for composition

### Firebase
- Use Firebase v9+ modular SDK
- Handle authentication states properly
- Use Firestore security rules (document them)
- Handle offline states gracefully
- Use proper Firestore data modeling (avoid deep nesting)

### API Integration
- Use async/await consistently
- Handle loading, success, and error states
- Implement proper request cancellation
- Use environment variables for API keys
- Never commit secrets

## Development Workflow

### Before Writing Code
- Understand the requirement fully
- Check if similar functionality exists
- Plan the component structure
- Consider edge cases and error states

### While Writing Code
- Write self-documenting code (clear variable/function names)
- Add comments for complex logic or non-obvious decisions
- Keep functions small and focused
- Extract magic numbers/strings to constants
- Use early returns to reduce nesting

### After Writing Code
- Check for console errors/warnings
- Verify TypeScript compiles without errors
- Test the feature manually
- Ensure responsive design works
- Check accessibility (keyboard navigation, screen readers)

## Performance Considerations

- Lazy load routes and heavy components
- Optimize images and assets
- Minimize bundle size (check imports, avoid full library imports)
- Use React.memo, useMemo, useCallback judiciously (not everywhere)
- Monitor bundle size with tools like webpack-bundle-analyzer

## Security

- Never expose API keys or secrets in client code
- Validate and sanitize user inputs
- Use Firebase security rules
- Implement proper authentication checks
- Follow OWASP guidelines for web security

## Accessibility

- Use semantic HTML
- Ensure keyboard navigation works
- Add proper ARIA labels where needed
- Maintain focus management
- Test with screen readers
- Ensure color contrast meets WCAG AA standards

## Code Review Guidelines

When suggesting changes:
- Be specific about what needs to change and why
- Suggest concrete improvements, not just "this is wrong"
- Consider the MVP context (don't over-engineer)
- Point out potential bugs or edge cases
- Suggest performance improvements when relevant

## Common Patterns

### API Calls
```typescript
// Use this pattern for API calls
const fetchData = async (): Promise<Data> => {
  try {
    const response = await api.getData();
    return response.data;
  } catch (error) {
    console.error('Failed to fetch data:', error);
    throw error; // Re-throw for caller to handle
  }
};
```

### Component Structure
```typescript
// Component with proper TypeScript and error handling
interface ComponentProps {
  id: string;
  onAction: (id: string) => void;
}

export const Component: React.FC<ComponentProps> = ({ id, onAction }) => {
  const [loading, setLoading] = useState(false);
  const [error, setError] = useState<string | null>(null);

  // Component logic here

  if (loading) return <LoadingSpinner />;
  if (error) return <ErrorMessage message={error} />;

  return (
    // Component JSX
  );
};
```

## MVP-Specific Guidelines

- **Ship Fast, Iterate Faster**: Get working features out quickly, then refine
- **User Value First**: Focus on features that deliver immediate user value
- **Document Technical Debt**: If you make a shortcut, document it with a TODO and reason
- **Keep It Simple**: Prefer simple solutions over complex ones
- **Measure Everything**: Instrument key user actions (but don't over-instrument)

## What NOT to Do

- Don't create abstractions you don't need yet
- Don't optimize prematurely
- Don't skip error handling "for now"
- Don't use `any` to silence TypeScript errors
- Don't commit commented-out code
- Don't skip accessibility considerations
- Don't ignore TypeScript errors
- Don't create components that are too generic too early

## When You're Stuck

- Check existing codebase for similar patterns
- Review this rules file
- Consider the MVP scope - is this necessary?
- Ask: "What's the simplest thing that could work?"
- Document decisions and trade-offs

---

**Remember**: This is an MVP. Balance speed with quality. Write code that's good enough to ship and iterate on, but maintainable enough to build upon.
```

---

**Instructions**: Copy this content into a `.cursorrules` file in your project root. Customize the sections based on your specific needs and technology stack choices.
