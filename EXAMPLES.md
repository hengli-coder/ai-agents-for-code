# Usage Examples

This document provides practical examples of how to use the agent prompts in this repository.

## Example 1: Getting a Code Review

**Scenario**: You've written a Python function and want feedback.

**How to use**:
1. Use the [Code Review prompt](prompts/general/code-review.md)
2. Combine with [Python Best Practices](prompts/python/python-best-practices.md)

**Example interaction**:
```
Context: Use the code review prompt from prompts/general/code-review.md 
and Python best practices from prompts/python/python-best-practices.md

Please review this Python function:

def calc(a, b, op):
    if op == '+':
        return a + b
    elif op == '-':
        return a - b
    elif op == '*':
        return a * b
    else:
        return a / b
```

## Example 2: Fixing a Bug

**Scenario**: Your application has a null pointer exception.

**How to use**:
Use the [Bug Fix prompt](prompts/general/bug-fix.md)

**Example interaction**:
```
Context: Use the bug fix prompt from prompts/general/bug-fix.md

I'm getting a NullPointerException at line 45:
String result = user.getName().toUpperCase();

The error occurs when the user object exists but getName() returns null.
```

## Example 3: Refactoring Legacy Code

**Scenario**: You have a large function that needs to be broken down.

**How to use**:
Use the [Refactoring prompt](prompts/general/refactoring.md)

**Example interaction**:
```
Context: Use the refactoring prompt from prompts/general/refactoring.md

Please help refactor this 200-line function that handles user registration,
validation, email sending, and database updates all in one place.

[Paste your large function here]
```

## Example 4: Writing Tests

**Scenario**: You need to write unit tests for a new feature.

**How to use**:
1. Use the [Testing prompt](prompts/general/testing.md)
2. Combine with language-specific prompt for your tech stack

**Example interaction**:
```
Context: Use the testing prompt from prompts/general/testing.md
and JavaScript best practices from prompts/javascript/javascript-best-practices.md

Please help me write comprehensive tests for this authentication service:

class AuthService {
  async login(username, password) {
    // implementation
  }
  
  async logout(token) {
    // implementation
  }
}
```

## Example 5: Designing an API

**Scenario**: You're building a REST API for a blog platform.

**How to use**:
Use the [API Design prompt](prompts/general/api-design.md)

**Example interaction**:
```
Context: Use the API design prompt from prompts/general/api-design.md

Help me design a RESTful API for a blog platform that needs to:
- Manage posts (CRUD operations)
- Handle comments on posts
- Support user authentication
- Allow filtering and pagination
```

## Example 6: Security Audit

**Scenario**: You want to ensure your code is secure before deploying.

**How to use**:
Use the [Security prompt](prompts/general/security.md)

**Example interaction**:
```
Context: Use the security prompt from prompts/general/security.md

Please review this login endpoint for security vulnerabilities:

@app.route('/login', methods=['POST'])
def login():
    username = request.form['username']
    password = request.form['password']
    query = f"SELECT * FROM users WHERE username='{username}' AND password='{password}'"
    user = db.execute(query)
    return jsonify(user)
```

## Example 7: Writing Documentation

**Scenario**: You need to document a complex library function.

**How to use**:
1. Use the [Documentation prompt](prompts/general/documentation.md)
2. Combine with language-specific conventions

**Example interaction**:
```
Context: Use the documentation prompt from prompts/general/documentation.md
and Python best practices from prompts/python/python-best-practices.md

Please help me write comprehensive documentation for this function:

def process_data(data, filters=None, transform=True, output_format='json'):
    # Complex data processing logic
    pass
```

## Tips for Best Results

1. **Be Specific**: Provide clear context about what you're trying to achieve
2. **Include Code**: Share the actual code when relevant
3. **Mention Constraints**: Note any limitations or requirements
4. **Combine Prompts**: Use multiple prompts for comprehensive assistance
5. **Iterate**: Refine based on initial feedback

## Advanced Usage

### Combining Multiple Prompts

For comprehensive assistance, combine prompts strategically:

- **Code Review + Security**: For security-focused code reviews
- **Language-Specific + Testing**: For test-driven development
- **Refactoring + Documentation**: When improving and documenting code
- **API Design + Security**: For secure API development

### Example of Combined Usage:
```
Context: Use prompts from:
1. prompts/java/java-best-practices.md
2. prompts/general/testing.md
3. prompts/general/security.md

I'm developing a payment processing service in Java. Please help me:
1. Ensure the code follows Java best practices
2. Write comprehensive tests
3. Check for security vulnerabilities
```

## Getting Started

1. Browse the [Prompt Index](prompts/INDEX.md) to find relevant prompts
2. Choose the prompt(s) that match your task
3. Provide context and your code/question
4. Follow the guidance provided by the AI agent
5. Iterate as needed

For more information, see the main [README.md](README.md).
