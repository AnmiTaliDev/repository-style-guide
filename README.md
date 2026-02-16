# Repository Style Guide

A comprehensive guide to creating beautiful and professional repositories with proper documentation, structure, and conventions.

## Overview

This guide covers best practices for repository organization, file naming, documentation, and project structure. Whether you're starting a new project or improving an existing one, this guide will help you create professional, maintainable repositories.

## Documentation Structure

- **[Core Files](docs/core-files.md)** - Mandatory files: README and LICENSE
- **[Contribution Files](docs/contribution.md)** - CONTRIBUTING, CHANGELOG, AUTHORS
- **[Governance](docs/governance.md)** - CODE_OF_CONDUCT, SUPPORT, GOVERNANCE
- **[Legal & Security](docs/legal.md)** - SECURITY, PRIVACY, TRADEMARK, DCO, CLA, NOTICE
- **[Academic Projects](docs/academic.md)** - CITATION, ADOPTERS, MANIFESTO
- **[Installation & Build Guides](docs/guides.md)** - INSTALL, BUILD, DEPENDENCIES, GUIDE
- **[Configuration Files](docs/configuration.md)** - Git, Docker, Editor configs
- **[Additional Documentation](docs/additional.md)** - FAQ, EXAMPLES, ARCHITECTURE, API, MIGRATION, VERSION, FUNDING, CODEOWNERS
- **[Naming Conventions](docs/naming-conventions.md)** - File formats, naming standards, and synonyms

## Quick Start

### Essential Files (Every Repository)

1. **README.md** - ✅ Use markup (.md, .rst, .tex), ❌ never plain .txt
2. **LICENSE** - Required for all projects (MIT, Apache-2.0, GPL-3.0, etc.)

### Recommended Files (Growing Projects)

3. **CONTRIBUTING.md** - How to contribute
4. **CHANGELOG.md** - Track changes between versions
5. **CODE_OF_CONDUCT.md** - Community standards (use Contributor Covenant)
6. **SECURITY.md** - How to report vulnerabilities

### Advanced Files (Large/Complex Projects)

7. **GOVERNANCE.md** - Decision-making processes
8. **CITATION.md** or **CITATION.cff** - For academic/research projects
9. **ROADMAP.md** - Future plans
10. **ARCHITECTURE.md** - System design and structure

## Key Principles

1. **Use Markup Formats** - Always use .md, .rst, or .tex instead of .txt
2. **UPPER_CASE Convention** - Standard for documentation files (README.md, LICENSE, CONTRIBUTING.md)
3. **Be Consistent** - Pick naming conventions and stick to them
4. **Make It Discoverable** - Link important files from README
5. **Keep It Updated** - Outdated documentation is worse than no documentation

## Configuration Files

Don't forget essential configuration files:

- `.gitignore` - Exclude build artifacts and secrets
- `.editorconfig` - Consistent formatting across editors
- `.gitattributes` - Line ending and diff settings
- `.dockerignore` - For Docker projects

## License

This guide is licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](LICENSE).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to suggest improvements to this guide.

---

**Note:** This guide uses UPPER_CASE naming convention for documentation files, which is the most common standard in open source projects.
