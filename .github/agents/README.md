# Custom Agent Profiles

This directory contains custom agent profiles optimized for specific development tasks. These profiles provide specialized expertise and context for GitHub Copilot agents.

## Available Agents

### 🏗️ Architecture Agent (`architecture.md`)
Expert in software architecture and system design.

**Use for:**
- Designing new features or systems
- Reviewing architectural decisions
- Creating architectural diagrams
- Selecting appropriate design patterns
- Planning system scalability

**Example usage:**
```
@workspace /agent architecture.md Design a plugin system for the application
```

### 🧪 Test Agent (`test.md`)
Expert in testing strategies and test implementation.

**Use for:**
- Writing unit, integration, and end-to-end tests
- Improving test coverage
- Debugging test failures
- Designing testing strategies
- Implementing test fixtures and mocks

**Example usage:**
```
@workspace /agent test.md Write comprehensive tests for the authentication module
```

### 🐛 Debug Agent (`debug.md`)
Expert in debugging and troubleshooting issues.

**Use for:**
- Diagnosing and fixing bugs
- Analyzing error messages and stack traces
- Performance debugging
- Memory leak investigation
- Root cause analysis

**Example usage:**
```
@workspace /agent debug.md Help me debug why the API request is timing out
```

### 📚 Documentation Agent (`documentation.md`)
Expert in technical writing and documentation.

**Use for:**
- Writing README files
- Creating API documentation
- Writing user guides
- Documenting code with docstrings
- Creating tutorials and examples

**Example usage:**
```
@workspace /agent documentation.md Create comprehensive documentation for the new feature
```

## How to Use Custom Agents

1. **Via GitHub Copilot Chat:**
   - Use the `@workspace` command followed by `/agent <profile>.md`
   - Provide your specific request or question

2. **Best Practices:**
   - Choose the most relevant agent for your task
   - Provide clear, specific requests
   - Include necessary context and background
   - Review and validate agent suggestions
   - Iterate with follow-up questions if needed

3. **Combining Agents:**
   You can use multiple agents sequentially for complex tasks:
   - Architecture agent to design the feature
   - Test agent to create tests
   - Documentation agent to document the implementation

## Creating New Agents

To create a new custom agent profile:

1. Create a new `.md` file in this directory
2. Define the agent's expertise and responsibilities
3. Include guidelines and best practices
4. Provide examples and templates
5. Update this README with the new agent

## Agent Profile Structure

Each agent profile should include:
- **Primary Responsibilities**: What the agent specializes in
- **Guidelines**: How the agent approaches tasks
- **Best Practices**: Recommended patterns and approaches
- **Tools & Techniques**: Specific tools the agent leverages
- **Examples**: Sample code or approaches when applicable

## Notes

- These agents are optimized for Python projects but can adapt to other contexts
- Always review and validate agent-generated content
- Agents work best with clear, specific requests
- Keep agent profiles up-to-date as best practices evolve
