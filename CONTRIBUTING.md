# Contributing to my-ai-agent

Thank you for your interest in contributing to my-ai-agent! This document provides guidelines and instructions for contributing.

## 🎯 Code of Conduct

Be respectful, inclusive, and constructive in all interactions.

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- npm or yarn
- Git

### Setup Development Environment

```bash
# Clone the repository
git clone https://github.com/Danny-ai-team/my-ai-agent.git
cd my-ai-agent

# Install dependencies
npm install

# Create .env file (if needed)
cp .env.example .env

# Verify setup
npm run lint
```

## 📋 Development Workflow

### 1. Create a Feature Branch
```bash
git checkout -b feature/your-feature-name
# or for bugs:
git checkout -b fix/bug-description
```

### 2. Make Your Changes
- Follow the existing code style
- Add comments for complex logic
- Keep functions small and focused
- Add tests for new features

### 3. Test Your Changes
```bash
npm run lint      # Check code style
npm run test      # Run tests (when available)
npm run build     # Build for production
```

### 4. Commit Your Changes
```bash
git commit -m "feat: add new agent capability"
git commit -m "fix: resolve agent initialization issue"
git commit -m "docs: update API documentation"
```

Use these prefixes:
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation
- `style:` - Code style changes
- `refactor:` - Code refactoring
- `test:` - Adding tests
- `chore:` - Build, dependencies, etc.

### 5. Push and Create Pull Request
```bash
git push origin feature/your-feature-name
```

Then create a PR on GitHub with:
- Clear title: "Add [feature name]"
- Description of changes
- Reference to related issues (if any)

## 🏗️ Project Structure

```
src/
├── agents/          # AI agent implementations
├── core/            # Core framework code
├── utils/           # Utility functions
└── types/           # TypeScript type definitions

tests/
├── agents/          # Agent tests
└── core/            # Framework tests

docs/                # Documentation
AGENTS.md            # Agent specifications
```

## 📝 Commit Message Guidelines

Good commit messages help maintain project history:

```
feat: add memory management for conversation context

- Implement conversation history storage
- Add memory retention policies
- Include tests for memory edge cases

Fixes #42
```

## 🧪 Testing

Before submitting a PR:

```bash
# Run all tests
npm run test

# Run tests in watch mode
npm run test:watch

# Run specific test
npm run test -- agents.test.js

# Generate coverage report
npm run test:coverage
```

## 🔍 Code Review

Your PR will be reviewed for:
- ✅ Functionality - Does it work correctly?
- ✅ Code Quality - Is it well-written and maintainable?
- ✅ Tests - Are there adequate tests?
- ✅ Documentation - Is it documented?
- ✅ Performance - Are there any performance concerns?

## 📖 Documentation

- Update README.md for user-facing changes
- Update AGENTS.md for agent specifications
- Add JSDoc comments to functions
- Include examples for new features

Example JSDoc:
```javascript
/**
 * Initialize an AI agent with the given configuration
 * @param {Object} config - Agent configuration
 * @param {string} config.name - Agent name
 * @param {string} config.model - LLM model to use
 * @returns {Agent} Initialized agent instance
 * @throws {Error} If configuration is invalid
 */
function createAgent(config) {
  // implementation
}
```

## 🐛 Bug Reports

Found a bug? Please create an issue with:
- **Title:** Clear, descriptive title
- **Description:** What's happening?
- **Steps to Reproduce:** How to trigger the bug
- **Expected Behavior:** What should happen
- **Actual Behavior:** What actually happens
- **Environment:** Node version, OS, etc.

Example:
```markdown
## Title
Agent fails to initialize with custom model

## Steps to Reproduce
1. Create agent with model: "gpt-4-turbo"
2. Call agent.init()
3. Check console

## Expected
Agent initializes successfully

## Actual
TypeError: Cannot read property 'key' of undefined

## Environment
- Node.js 18.12.0
- OS: macOS 13.1
```

## 💡 Feature Requests

Have an idea? Open an issue with:
- **Title:** Feature idea
- **Description:** What problem does it solve?
- **Use Case:** How would it be used?
- **Examples:** Code examples if applicable

## ✅ PR Checklist

Before submitting your PR, ensure:
- [ ] Code follows project style guide
- [ ] All tests pass locally (`npm run test`)
- [ ] Code is well-commented
- [ ] Documentation is updated
- [ ] No console.log or debug code left
- [ ] Commit messages are clear
- [ ] PR description explains changes

## 🎓 Learning Resources

- [JavaScript Best Practices](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)
- [Node.js Documentation](https://nodejs.org/en/docs/)
- [Git Workflow Guide](https://guides.github.com/)

## 🤝 Need Help?

- Check existing issues and discussions
- Ask in GitHub Discussions
- Review similar code in the repository
- Open an issue if stuck

## 🙏 Thank You!

Your contributions help make my-ai-agent better for everyone. We appreciate your time and effort!

---

**Happy coding!** 🚀
