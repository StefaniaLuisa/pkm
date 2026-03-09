
# GitHub Copilot Instructions for Engaging Networks Regive

## Project Overview

Engaging Networks Regive is a standalone component that creates a customizable One-Click Instant Donation UX on "Thank You" pages for Engaging Networks donation forms. It allows donors to make an additional donation with a single click without having to fill out the entire form again.

The component works by:

1. On first page: Capturing transaction tokens (securely) if the user has made a donation
2. On thank you page: Showing a customizable UI with donation amount options
3. On click: Submitting a second donation using the stored tokens information

## Tech Stack

- **TypeScript** - Core language for type safety and maintainability
- **SCSS** - Styling with nested selectors and variables
- **Vite** - Build tool for producing the final JS distribution
- **Vanilla JS/DOM** - No heavy frameworks, just plain JavaScript DOM manipulation
- **No dependencies** - Self-contained with no external runtime dependencies

## Project Structure

```plaintext
src/
├── main.ts                    # Entry point
├── style.scss                 # Global styles for the component
└── lib/
    ├── regive.ts              # Main component class
    ├── regive-options.ts      # Configuration interface
    ├── engrid.ts              # Engaging Networks utilities
    └── confetti.js            # Confetti animation implementation
```

## Key Concepts

### Core Classes

- **Regive**: Main class that handles initialization, detecting page types, and UI management. Responsible for the component's lifecycle.
- **ENGrid**: Utility class for interacting with Engaging Networks forms, fields and page information.
- **RegiveOptions**: TypeScript interface defining all available configuration options.
- **RegiveConfetti**: Handles the celebration animation when donations complete.

### Component Lifecycle

1. **Initialization**: Script loads, creates Regive instance, detects page type
2. **First Page**: 
   - If not embedded: watches for token fields and saves values to localStorage
   - If embedded: hides the form and shows a custom banner with amount buttons
3. **Thank You Page**: 
   - If not embedded: replaces `<regive>` tag with an iframe
   - If embedded: shows donation success UI and triggers confetti

### Communication

- Parent-Child communication happens via postMessage
- Custom events include: loaded, height, celebrate, success, reset

## Coding Guidelines

### Naming Conventions

- Use camelCase for variables and methods
- Use PascalCase for classes and interfaces
- Use descriptive names that reflect purpose

### TypeScript Best Practices

- Always use proper type definitions
- Avoid `any` type when possible
- Use optional chaining (`?.`) for potentially undefined values
- Use nullish coalescing (`??`) for fallback values

### CSS Practices

- Use BEM-like naming (block__element--modifier)
- Prefix classes with `regive-` to avoid conflicts
- Use data attributes for state (`data-theme`, etc.)
- Utilize CSS variables for theming

## Common Tasks

### Adding a New Configuration Option

1. Add the option to `RegiveOptions` interface in `regive-options.ts`
2. Add implementation in `regive.ts`
3. Add default value handling
4. Update documentation in [README.md](http://README.md)

### Adding a New Theme

1. Add the theme name to the `themes` array in `regive.ts`
2. Add theme-specific styles in `style.scss`
3. Update documentation in [README.md](http://README.md)

### Debugging Tips

- Use the `log()` method in the Regive class
- Enable debug mode with `?debug` in script URL
- Check browser console for detailed logs
- Use test mode (`test="true"`) for simulating donations

### Building and Testing

1. Run development server with `npm run dev`
2. Test in browser at `http://localhost:3000`
3. Build production version with `npm run build:prod`
4. The output file will be at `dist/regive.min.js`

## Security Considerations

- Component handles "tokens" from VGS, not actual credit card data
- Always use HTTPS for secure communication
- Keep debug mode disabled in production

## Feature Enhancement Guidelines

When adding new features, consider:

1. Will this work across different Engaging Networks clients?
2. Does it maintain backward compatibility?
3. Is it properly documented?
4. Does it follow the established patterns and conventions?
5. Is it accessible?