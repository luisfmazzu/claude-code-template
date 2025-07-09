# Full-Stack Coding Interview AI Instructions

## Tool Setup

### Primary Tool
- **Claude Code** - Selected for superior context handling (July 8th, 2025)
- **Custom Project Rules** - Modified `CLAUDE.md` with project-specific instructions

### Model Control Protocol (MCP) Extensions
- **Context7** - Enhanced context management  
  https://github.com/upstash/context7
- **Shadcn UI** - Component library integration  
  https://mcpservers.org/servers/heilgar/shadcn-ui-mcp-server
- **Supabase** - Database and backend services  
  https://supabase.com/docs/guides/getting-started/mcp?queryGroups=os&os=linux#claude-code
- **Github MCP** - PR automation  
  https://github.com/github/github-mcp-server
- **TaskMaster** - Task management  
  https://www.task-master.dev/
- **Playwright** - Testing framework  
  https://github.com/microsoft/playwright-mcp

### Future MCP Integrations
- **Mem0** - Requires local server setup - Ideal for maintenance later on  
  https://github.com/mem0ai/mem0-mcp
- **Vercel** - Deployment management  
  https://github.com/nganiet/mcp-vercel


## Development Workflow

### Phase 1: Planning
1. Switch to planning mode
2. Change model to Claude Opus: `/model opus`
3. Send prompt from `AI-PROMPT.md`
4. When plan is ready, select "2" to "keep planning" (do not implement yet)

### Phase 2: Implementation
1. Change model to Claude Sonnet: `/model sonnet`
2. List all tasks and sub-tasks
3. Begin task execution cycle

### Development Cycle
Each iteration should include:
- **Implement** the next task
- **Test** functionality when possible
- **Review** code thoroughly

## Technical Challenges Encountered

### 1. Context Management
- **Challenge**: Large codebases can exceed AI context limits
- **Solution**: Use Context7 MCP for enhanced context management

### 2. Testing Integration
- **Challenge**: Ensuring comprehensive test coverage across different frameworks
- **Solution**: Implement Playwright MCP for end-to-end testing

### 3. Scalability Concerns
- **Limitation**: Current AI models cannot handle scalability review without human oversight
- **Recommendation**: Full human review required for production-ready scalability

### 4. Code Quality Consistency
- **Challenge**: Maintaining consistent code style across large projects
- **Solution**: Implement strict TypeScript rules and automated linting

## Best Practices

### Code Organization
- Follow the established project structure in `CLAUDE.md`
- Use feature-based module organization
- Implement proper separation of concerns

### Development Process
- Always commit frequently using GitHub MCP
- Create detailed task breakdowns with TaskMaster
- Test thoroughly before moving to next task
- Create pull requests for major feature completions

### Quality Assurance
- Run all tests before committing
- Use TypeScript strict mode
- Follow established coding conventions
- Implement proper error handling