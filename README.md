# AI Agents for Code

A comprehensive repository for managing AI agent prompts that help developers write better code. This collection includes prompts for code review, bug fixing, refactoring, documentation, and language-specific best practices.

## Quick Start

1. **Browse Prompts**: Check the [Prompt Index](prompts/INDEX.md) to find what you need
2. **Choose Your Task**: Select from code review, bug fixing, testing, documentation, etc.
3. **Use with AI**: Provide the prompt to your AI assistant along with your code
4. **See Examples**: Visit [EXAMPLES.md](EXAMPLES.md) for practical usage examples

## Overview

This repository provides structured prompts for AI agents to assist with various coding tasks. Each prompt is designed to guide AI agents in helping developers with specific programming challenges.

## Repository Structure

```
prompts/
├── general/           # General-purpose coding prompts
│   ├── code-review.md       # Code review guidelines
│   ├── bug-fix.md           # Bug fixing assistance
│   ├── refactoring.md       # Code refactoring guidance
│   └── documentation.md     # Documentation writing
├── python/            # Python-specific prompts
│   └── python-best-practices.md
├── javascript/        # JavaScript-specific prompts
│   └── javascript-best-practices.md
└── java/             # Java-specific prompts
    └── java-best-practices.md
```

## Available Prompts

### General Prompts

- **Code Review** (`prompts/general/code-review.md`)
  - Expert code review focusing on quality, bugs, performance, and security
  - Provides structured feedback with actionable suggestions

- **Bug Fix** (`prompts/general/bug-fix.md`)
  - Systematic approach to identifying and fixing bugs
  - Includes root cause analysis and prevention strategies

- **Refactoring** (`prompts/general/refactoring.md`)
  - Guide for improving code structure and maintainability
  - Follows best practices and SOLID principles

- **Documentation** (`prompts/general/documentation.md`)
  - Comprehensive documentation writing guidelines
  - Covers API docs, examples, and usage instructions

### Language-Specific Prompts

- **Python** (`prompts/python/python-best-practices.md`)
  - PEP standards and modern Python features
  - Type hints, docstrings, and pythonic patterns

- **JavaScript** (`prompts/javascript/javascript-best-practices.md`)
  - ES6+ features and modern JavaScript practices
  - Async/await, modules, and TypeScript considerations

- **Java** (`prompts/java/java-best-practices.md`)
  - Modern Java features and enterprise patterns
  - SOLID principles and design patterns

## How to Use

1. **Choose a Prompt**: Select the appropriate prompt based on your task
2. **Provide Context**: Give the AI agent the prompt along with your code/requirements
3. **Get Assistance**: The AI agent will follow the guidelines to help you
4. **Iterate**: Refine based on the agent's suggestions

### Example Usage

```
Use the prompt from prompts/general/code-review.md to review this code:
[Your code here]
```

For more detailed examples and use cases, see [EXAMPLES.md](EXAMPLES.md)

## Contributing

To add new prompts or improve existing ones:

1. Follow the existing format and structure
2. Include clear role definition, task description, and guidelines
3. Provide output format expectations
4. Add examples when helpful

## Prompt Template

Each prompt should include:

```markdown
# [Prompt Name] Agent Prompt

## Role
[Define the AI agent's expertise]

## Task
[Describe what the agent should help with]

## Guidelines
[Specific rules and best practices]

## Output Format
[Expected structure of the response]
```

## Best Practices for Writing Prompts

- Be specific and clear about the agent's role
- Provide concrete guidelines and examples
- Define expected output format
- Include relevant best practices
- Keep prompts focused on specific tasks
- Update prompts based on feedback and results

## License

Apache License 2.0 - See LICENSE file for details
