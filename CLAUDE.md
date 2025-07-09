# Project Setup Instructions

## Technology Stack

- **Frontend Framework**: Next.js with TypeScript
- **Build Tool**: npm
- **Styling**: Tailwind CSS
- **Backend**: Nest.js with TypeScript, Supabase

## Development Setup

### Frontend Project Structure

```
src/
├── components/     # React components
├── pages/         # Page components
├── hooks/         # Custom React hooks
├── utils/         # Utility functions
├── types/         # TypeScript type definitions
├── lib/           # Third-party library configurations
│   └── supabase.ts # Supabase client setup
└── styles/        # Global styles and Tailwind config
```

### Backend Project Structure

```
src/
├── modules/       # Feature modules
├── common/        # Shared utilities and configurations
├── config/        # Configuration files
├── database/      # Database-related files
```

## MCPs

Use existing connected MCPs accordingly and whenever you can. Here is how you should use each of them:

### Context7

- The MCP pulls up-to-date, version-specific documentation and code examples straight from the source.
- Use it for all technical tasks, mainly for implementations and planning stages where technical decisions are required.

### taskmaster-ai

- Use it to plan all tasks and sub-tasks.
- Always be detailed when writing tasks and memorize descriptions.
 
### Playwright MCP

- When given a URL link, use playwright MCP to get the content or design of the page before continuing.

### Shad CN UI

- Use Shad CN MCP to get components and designs for the frontend when you have freedom of creativity.

### GitHub MCP

- Use GitHub MCP to add commits to Git often (at least once every sub-task).
- Create a Pull Request in GitHub after finishing a task

### Databases MCP

- Use Supabase MCP to setup PostgreSQL servers or the MongoDB MCP for NoSQL servers (mongo).

## Development Guidelines

### TypeScript

- Use strict mode for type safety
- Define interfaces for all data models
- Avoid using `any` type

### React Best Practices

- Use functional components with hooks
- Implement proper error boundaries
- Keep components small and focused
- Use React.memo for performance optimization when needed

### Tailwind CSS

- Use utility classes for styling
- Create custom components for repeated patterns
- Configure theme in `tailwind.config.js`

### State Management

- Use React Context for simple global state
- Consider React Query for server state
- Consider Zustand for complex state management
- Keep component state local when possible
- Avoid prop drilling by leveraging state management tools

### Implementing a task

- Review existing documents and the current architecture
- Review sub-tasks and minimal details for the task
- Implement the task from beginning to end
- Review if the task was throughly completed
- Write unit and integration tests
- Validate if all test pass before moving on to the next task
- If everything is complete, create a Pull Request in GitHub with the changes.