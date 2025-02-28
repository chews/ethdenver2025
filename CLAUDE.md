# ETHDenver 2025 Project Guide

## Commands
- **Build**: `npm run build`
- **Dev server**: `npm run dev`
- **Tests**: `npm test`
- **Single test**: `npm test -- -t "test name"`
- **Lint**: `npm run lint`
- **Format**: `npm run format`
- **Typecheck**: `npm run typecheck`

## Code Style Guidelines
- **Formatting**: Use Prettier with default configuration
- **Types**: Prefer TypeScript with strict type checking enabled
- **Naming**: 
  - camelCase for variables and functions
  - PascalCase for components and classes
  - UPPER_SNAKE_CASE for constants
- **Imports**: Group imports (React, external libs, internal), sort alphabetically
- **Components**: Function components with hooks preferred over class components
- **Error Handling**: Use try/catch for async operations, proper error logging
- **State Management**: Use React Context for global state where appropriate
- **Comments**: JSDoc for exported functions and components

## Architecture Notes
- Follow component-based architecture
- Keep components small and focused on single responsibility
- Separate UI components from business logic