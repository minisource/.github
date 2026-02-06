# Contributing to Minisource

Thank you for considering contributing to Minisource! We welcome contributions from everyone.

## Code of Conduct

By participating in this project, you agree to maintain a respectful and inclusive environment for everyone.

## How Can I Contribute?

### 🐛 Reporting Bugs

Before creating a bug report:
1. Check if the issue already exists
2. Verify you're using the latest version
3. Collect relevant information (logs, environment, steps to reproduce)

When creating a bug report, use the issue template and include:
- Clear, descriptive title
- Detailed steps to reproduce
- Expected vs actual behavior
- Screenshots or logs (if applicable)
- Environment details (OS, versions, etc.)

### 💡 Suggesting Features

Feature suggestions are welcome! Use the feature request template and include:
- Problem you're trying to solve
- Proposed solution
- Alternative solutions considered
- Any mockups or examples

### 🔧 Pull Requests

#### Before You Start

1. **Check existing issues/PRs** - Someone might already be working on it
2. **Open an issue first** - For significant changes, discuss the approach
3. **Fork the repository** - Work on your own fork

#### Development Setup

Each repository has its own setup instructions in its README. Generally:

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/REPO_NAME
cd REPO_NAME

# Create a feature branch
git checkout -b feature/your-feature-name

# Install dependencies (depends on project type)
# Go projects
go mod download

# .NET projects
dotnet restore

# Node/Next.js projects
npm install
```

#### Making Changes

1. **Follow the existing code style**
   - Go: `gofmt`, `golangci-lint`
   - .NET: EditorConfig, StyleCop
   - JavaScript/TypeScript: ESLint, Prettier

2. **Write meaningful commit messages**
   ```
   feat: add user authentication endpoint
   fix: resolve null pointer in storage service
   docs: update API documentation
   test: add integration tests for payment flow
   ```

   Use conventional commits: `type(scope): description`
   - `feat`: New feature
   - `fix`: Bug fix
   - `docs`: Documentation
   - `test`: Tests
   - `refactor`: Code refactoring
   - `chore`: Maintenance tasks

3. **Add tests**
   - Unit tests for new functionality
   - Update existing tests if behavior changes
   - Ensure all tests pass locally

4. **Update documentation**
   - Update README if adding features
   - Add/update API documentation
   - Include code comments for complex logic

#### Submitting a Pull Request

1. **Push your branch**
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create the PR**
   - Use a clear, descriptive title
   - Fill out the PR template completely
   - Link related issues
   - Add screenshots/demos if applicable

3. **Review Process**
   - Address review comments promptly
   - Keep the PR focused (one feature/fix per PR)
   - Ensure CI checks pass
   - Squash commits if requested

#### PR Requirements

- [ ] Code follows project style guidelines
- [ ] Self-reviewed the code
- [ ] Added/updated tests
- [ ] All tests pass locally
- [ ] Updated documentation
- [ ] No new warnings/errors
- [ ] Signed commits (optional but recommended)

## Project Structure

### Go Projects
```
cmd/          # Application entrypoints
internal/     # Private application code
pkg/          # Public library code
tests/        # Integration tests
docs/         # Documentation
```

### .NET Projects
```
src/          # Source code
tests/        # Unit and integration tests
docs/         # Documentation
```

### Next.js Projects
```
src/
  app/        # App router pages
  components/ # React components
  lib/        # Utilities
  api/        # API clients
tests/        # Tests
```

## Style Guides

### Go
- Follow [Effective Go](https://golang.org/doc/effective_go)
- Use `gofmt` for formatting
- Run `golangci-lint` before committing

### .NET
- Follow [.NET coding conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions)
- Use `dotnet format`

### TypeScript/JavaScript
- Use ESLint and Prettier
- Follow Airbnb style guide
- Prefer functional components and hooks

## Testing

- Write unit tests for business logic
- Add integration tests for API endpoints
- Ensure >80% code coverage for new code
- Use meaningful test descriptions

### Running Tests

```bash
# Go
go test ./...

# .NET
dotnet test

# Node.js
npm test
```

## Documentation

- Document public APIs
- Add inline comments for complex logic
- Update README for new features
- Include examples in documentation

## Questions?

If you have questions:
1. Check the repository's README
2. Search existing issues
3. Open a new discussion or issue

## Recognition

Contributors are recognized in:
- Release notes
- Contributors section
- Acknowledgments in documentation

Thank you for contributing to Minisource! 🎉
