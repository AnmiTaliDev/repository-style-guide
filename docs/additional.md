# Additional Documentation Files

Optional but highly valuable files that improve project quality and user experience.

## FAQ

Frequently Asked Questions - saves time for both users and maintainers.

### Required Contents
- Common questions from users with clear answers
- Troubleshooting tips for known issues
- Explanation of design decisions
- Comparison with similar tools or alternatives
- Performance-related questions
- Licensing and usage questions
- Platform compatibility questions
- Known limitations and workarounds

### When to Include
- After receiving repeated questions
- For complex projects with learning curve
- Projects with common pitfalls or gotchas
- Do NOT create empty FAQ preemptively

### Naming Variants
- `FAQ.md`
- `FAQ`

### Organization
- Group by topic or category
- Most common questions first
- Clear question and answer format
- Link to relevant documentation for details

## EXAMPLES

Usage patterns and code demonstrations.

### Structure Options

**Single File Option:**
- All examples in one document
- Organized by complexity (basic to advanced)
- Clear section headers
- Brief explanations with each example

**Directory Option:**
- `examples/` directory with subdirectories
- Separate files for different use cases
- README in each subdirectory
- Runnable code files
- Sample data if needed

### Naming Variants
- `EXAMPLES.md` (single file)
- `EXAMPLES` (single file)
- `examples/` (directory, typically lowercase)

### Required Contents
- Basic usage examples
- Common use case demonstrations
- Advanced feature examples
- Real-world application scenarios
- Error handling demonstrations
- Configuration examples

### Best Practices
- Make examples runnable as-is
- Include comments explaining key points
- Start simple, progress to complex
- Cover common use cases
- Provide sample input/output data
- Keep examples updated with API changes

## ARCHITECTURE

High-level architecture and design documentation.

### Required Contents
- System architecture overview
- Component relationships and interactions
- Design patterns employed
- Key abstractions and their purposes
- Data flow through the system
- Rationale for major design decisions
- Technology choices and justifications
- Scalability considerations
- Security architecture
- Performance characteristics

### When to Include
- Complex projects with multiple components
- Frameworks and libraries
- Projects where understanding design is important for contributors
- Systems with non-obvious architecture
- Projects with specific architectural patterns

### Naming Variants
- `ARCHITECTURE.md`
- `ARCHITECTURE`
- `DESIGN.md`
- `DESIGN`

### Purpose
- Helps new contributors understand the big picture
- Documents architectural decisions
- Facilitates system reasoning
- Prevents architectural drift
- Onboarding resource

## API

API reference or documentation.

### Required Contents
- Endpoint documentation (for REST APIs)
- Function/class documentation (for libraries)
- Request/response formats
- Authentication mechanisms
- Authorization requirements
- Rate limiting information
- Error responses and codes
- Usage examples for each endpoint/function
- Versioning information
- Deprecation notices

### Modern Alternatives
Instead of manually maintained API.md:
- OpenAPI/Swagger specification files (`openapi.yaml`, `swagger.json`)
- Generated documentation from code comments (JSDoc, Sphinx, Doxygen, etc.)
- `docs/api/` directory for extensive documentation
- Interactive API documentation tools

### Naming Variants
- `API.md`
- `API`
- `API_REFERENCE.md`
- `openapi.yaml` (for REST APIs, preferred)
- `swagger.json` (for REST APIs)
- `docs/api/` (directory)

### When to Use API.md
- Simple APIs with few endpoints
- Quick reference documentation
- Not recommended for large APIs (use generated docs)

## MIGRATION

Guide for upgrading between major versions.

### Required Contents
- Breaking changes listed clearly
- Step-by-step migration instructions
- Code transformation examples (before/after)
- Deprecation warnings and timelines
- Support timeline for old versions
- Common migration pitfalls
- Automated migration tools (if available)
- Testing recommendations after migration
- Rollback procedures

### When to Include
- After releasing v2.0+ with breaking changes
- When API changes significantly
- Enterprise software with long-lived deployments
- Major refactoring or architectural changes
- Dependency version bumps with breaking changes

### Naming Variants
- `MIGRATION.md`
- `MIGRATION`
- `UPGRADING.md`
- `UPGRADING`

### Organization
- Separate section for each major version transition
- Chronological order (newest first)
- Clear headings for each breaking change
- Priority levels (must-do vs. recommended)

## VERSION

Current version identifier of the project.

### Content
- Single version number
- Optional: release date
- Optional: version name or codename

### Naming Variants
- `VERSION`
- `VERSION.txt`
- `.version`

### Modern Alternatives (Preferred)
Instead of VERSION file, use:
- Git tags for versioning
- Language-specific version fields:
  - Python: `__version__` in `__init__.py` or `pyproject.toml`
  - Node.js: `version` in `package.json`
  - Rust: `version` in `Cargo.toml`
  - Java: `pom.xml` or `build.gradle`

### When to Use VERSION File
- When no language-specific version file exists
- For language-agnostic projects
- When multiple version identifiers exist
- Not recommended for most modern projects

## FUNDING

Information about project funding and sponsorship.

### Required Contents
- How to sponsor or donate
- Available sponsorship platforms
- Current sponsors (with permission)
- What funding supports (development, infrastructure, etc.)
- Sponsorship tiers and benefits
- Tax deductibility information (if applicable)
- Transparency about fund usage

### GitHub Integration
GitHub recognizes `.github/FUNDING.yml` format:
- Adds "Sponsor" button to repository
- Supports multiple funding platforms
- Structured YAML format

### Naming Variants
- `FUNDING.md`
- `FUNDING`
- `FUNDING.yml` (in `.github/` directory, recommended for GitHub)
- `SPONSORS.md`

### Supported Platforms
- GitHub Sponsors
- Patreon
- Open Collective
- Ko-fi
- Tidelift
- Custom URLs

## CODEOWNERS

Automatically assigns reviewers for pull requests.

### Purpose
- Automatic reviewer assignment
- Define code ownership boundaries
- Ensure appropriate review
- Distribute review responsibilities
- Required reviews by designated owners

### File Format
- Comment lines start with `#`
- Patterns match files or directories
- Owner specified by GitHub username or team
- Most specific pattern takes precedence
- Supports glob patterns

### Required Location
Must be in one of these locations:
- Repository root: `CODEOWNERS`
- `.github/CODEOWNERS` (recommended)
- `docs/CODEOWNERS`

### When to Use
- Projects with multiple maintainers
- Code with clear ownership areas
- Organizations with defined teams
- Not necessary for solo projects

### Content Structure
- Global ownership patterns
- Directory-specific ownership
- File-specific ownership
- Team assignments
- Multiple owners per pattern

## Best Practices

1. **FAQ after questions arise** - Don't create empty FAQ preemptively
2. **Examples are invaluable** - Users learn best from examples
3. **ARCHITECTURE for complex projects** - Helps contributors understand
4. **MIGRATION for breaking changes** - Respect users' time and investment
5. **Use GitHub's FUNDING.yml** - Better integration than custom file
6. **CODEOWNERS for teams** - Automates review process
7. **Link from README** - Make all files discoverable
8. **Keep updated** - Outdated documentation worse than none
9. **API docs should be generated** - Manual API docs become stale
10. **VERSION in language-standard location** - Don't create custom files
