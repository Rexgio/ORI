# PROJECT.md — Project Knowledge Base

## 1. PROJECT OVERVIEW

**Name:** Ori Frontend

**Description:**
A Next.js frontend application built with React, TypeScript and Tailwind CSS for the Ori project. This is a modern web application using the App Router architecture.

**Current status:**
Development

**Main objectives:**

- Create a responsive and accessible user interface
- Implement clean component composition patterns 
- Ensure type safety with TypeScript
- Utilize Tailwind CSS for styling

## 2. TECHNOLOGY STACK

| Component       | Technology   | Version   |
| --------------- | ------------ | --------- |
| Language        | TypeScript   | 5.x       |
| Framework       | Next.js      | 16.4.6    |
| Runtime         | Bun          | 1.4.4     |
| Database        | None         | -         |
| Package manager | Bun          | 1.4.4     |
| Other           | React        | 19.3.0    |

## 3. ARCHITECTURE

The project uses Next.js App Router with the following structure:
- Components are organized in /app/ directory
- Uses React Server Components by default 
- Follows TypeScript interfaces for component props
- Utilizes Tailwind CSS for styling

### Main components

- Page components in /app/page.tsx
- Layout components in /app/layout.tsx
- Global styles in /app/globals.css
- Assets in /public/

### Data flow

Application state is managed through React's built-in state management patterns. Server components communicate with client components using props and state.

### External integrations

None at this time

## 4. PROJECT STRUCTURE

```text
ori-frontend/
├── app/                     # Next.js App Router pages and layout
│   ├── favicon.ico
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── public/                  # Static assets
├── src/                     # Source code (not present in this project)
├── tests/                   # Test files (not present in this project)
├── docs/                    # Documentation (not present in this project)
├── .gitignore
├── next.config.ts
├── package.json
├── tsconfig.json
└── README.md
```

## 5. DEVELOPMENT ENVIRONMENT

### Requirements

- Node.js >= 18 or Bun >= 1.4.4
- Git for version control

### Commands

| Action      | Command   |
| ----------- | --------- |
| Install     | `bun install` |
| Development | `bun dev` |
| Build       | `bun build` |
| Test        | `bun test` (not implemented) |
| Lint        | `bun lint` |
| Type check  | `bun tsc` or equivalent |

## 6. CODING CONVENTIONS

### Naming

- Use PascalCase for React component names
- Use kebab-case for file names (e.g., page.tsx)
- Use camelCase for variables and functions
- Use uppercase for constants

### Organization

- Components should be organized in /app/ directory structure
- Each route has its own folder with page.tsx, layout.tsx files
- Keep related components together

### Patterns

- Follow React component composition patterns
- Use TypeScript interfaces for props
- Leverage React's server/client component distinction appropriately

### Error handling

- Use React error boundaries when appropriate
- Handle async operations with proper loading states
- Display user-friendly error messages

### Testing

- Component testing using React Testing Library (not yet implemented)
- Integration tests in the future (planned)

## 7. IMPORTANT BUSINESS LOGIC

- Application renders a simple welcome page with links to documentation and deployment
- Uses Next.js's built-in font optimization
- Implements responsive design patterns
- Follows accessibility best practices

## 8. CONSTRAINTS

### Technical constraints

- Must use React Server Components (default in App Router)
- Must use TypeScript for type safety
- Must follow Tailwind CSS utility classes only 
- Cannot rely on external libraries without explicit approval

### Compatibility

- Works with modern browsers that support ES2020+ features
- Compatible with Next.js 16.4.6 and React 19.3.0

### Security

- No sensitive data handling at this time
- Follows CSP guidelines for secure script loading

### Things that must not change

- Core App Router file structure in /app/
- Basic page rendering flow from /app/page.tsx
- Global styling in /app/globals.css  
- TypeScript configuration (tsconfig.json)

## 9. CURRENT STATE

**Implemented:**

- Basic Next.js/React application setup
- TypeScript type checking configured 
- Tailwind CSS integration enabled
- Development server with hot reloading

**In progress:**

- Implementation of more complex UI components
- Integration of additional features
- Testing framework setup (planned)

**Known issues:**

- None at this time

**Pending work:**

- Add real application functionality beyond the default page
- Implement testing suite
- Optimize performance for production deployment

## 10. IMPORTANT DECISIONS

Record relevant architectural and technical decisions.

| Decision   | Reason   | Date   |
| ---------- | -------- | ------ |
| App Router | Modern Next.js approach with better performance and component composition | Nov 2024 |
| TypeScript | Ensures type safety for React components | Nov 2024 |
| Tailwind CSS | Fast styling with utility classes | Nov 2024 |

## 11. ADDITIONAL CONTEXT

This is a minimal Next.js starter project that can be extended to build the actual Ori application.

For this project, always consider:
- The App Router file structure in /app/
- React component composition patterns
- TypeScript interfaces for props and state
- Tailwind CSS utility classes for styling
- Server vs client components usage
