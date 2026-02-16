# Naming Conventions & File Synonyms

Guidelines for file naming, formats, and accepted synonyms in professional repositories.

## General Conventions

### Case Style
**Standard: UPPER_CASE**

```
✅ README.md
✅ LICENSE
✅ CONTRIBUTING.md
✅ CODE_OF_CONDUCT.md

❌ readme.md (acceptable but not standard)
❌ Readme.md (inconsistent)
❌ contributing.md (acceptable but not standard)
```

**Exceptions:**
- `docs/` - Typically lowercase
- `examples/` - Typically lowercase
- Language-specific files: `package.json`, `requirements.txt`, etc.
- Configuration files: `.gitignore`, `.editorconfig`, etc.

### File Formats

**Recommended:** Use markup formats, not plain text

```
✅ .md (Markdown) - Most common
✅ .rst (reStructuredText) - Common in Python
✅ .tex (LaTeX) - Academic projects
✅ .adoc (AsciiDoc) - Technical documentation

❌ .txt - Avoid
❌ No extension - Avoid (except LICENSE, which can be without extension)
```

### Underscores vs Hyphens
- **Standard:** Underscores (`_`)
- Examples: `CODE_OF_CONDUCT.md`, `PULL_REQUEST_TEMPLATE.md`
- Hyphens acceptable for formats: `LICENSE-GPL-3.0`

## Complete Synonym Reference

### README
```
README.md
README
README.rst
README.tex
readme.md
ReadMe.md
```

### LICENSE
```
LICENSE
LICENSE.md
LICENSE.txt
LICENSE-<license-name>           # e.g., LICENSE-GPL-3.0
LICENSE-<license-name>.md        # e.g., LICENSE-MIT.md
LICENCE                           # British spelling
LICENCE.md
COPYING
COPYING.md
```

### CHANGELOG
```
CHANGELOG.md
CHANGELOG
HISTORY.md
HISTORY
NEWS.md
NEWS
RELEASES.md
RELEASES
CHANGES.md
CHANGES
```

### CONTRIBUTING
```
CONTRIBUTING.md
CONTRIBUTING
HACKING.md
HACKING
DEVELOPMENT.md
DEVELOPMENT
```

### CODE_OF_CONDUCT
```
CODE_OF_CONDUCT.md
CODE_OF_CONDUCT
CONDUCT.md
CONDUCT
CoC.md
CoC
```

### SUPPORT
```
SUPPORT.md
SUPPORT
HELP.md
HELP
CONTACT.md
CONTACT
TROUBLESHOOTING.md
TROUBLESHOOTING
```

### GOVERNANCE
```
GOVERNANCE.md
GOVERNANCE
CHARTER.md
CHARTER
DECISIONS.md
DECISIONS
```

### AUTHORS / CONTRIBUTORS / MAINTAINERS
```
AUTHORS.md
AUTHORS
CONTRIBUTORS.md
CONTRIBUTORS
MAINTAINERS.md
MAINTAINERS
CREDITS.md
CREDITS
OWNERS
THANKS.md
THANKS
MEMBERS.md
MEMBERS
CORE_TEAM.md
CORE_TEAM
STEWARDS.md
STEWARDS
```

### ACKNOWLEDGMENTS
```
ACKNOWLEDGMENTS.md
ACKNOWLEDGMENTS
ACKNOWLEDGEMENTS.md      # British spelling
ACKNOWLEDGEMENTS
ATTRIBUTIONS.md
ATTRIBUTIONS
THANKS.md
THANKS
```

### SECURITY
```
SECURITY.md
SECURITY
VULNERABILITIES.md
VULNERABILITIES
SECURITY_POLICY.md
POLICY.md
```

### PRIVACY
```
PRIVACY.md
PRIVACY
PRIVACY_POLICY.md
DATA_USAGE.md
DATA_USAGE
GDPR.md
GDPR
```

### TRADEMARK
```
TRADEMARK.md
TRADEMARK
BRAND_GUIDELINES.md
BRAND_GUIDELINES
LOGO.md
LOGO
BRANDING.md
BRANDING
```

### NOTICE
```
NOTICE
NOTICE.md
LEGAL.md
LEGAL
DISCLAIMER.md
DISCLAIMER
```

### DCO
```
DCO
DCO.md
DEVELOPER_CERTIFICATE.md
DEVELOPER_CERTIFICATE_OF_ORIGIN.md
```

### CLA
```
CLA.md
CLA
CONTRIBUTOR_LICENSE_AGREEMENT.md
CONTRIBUTOR_LICENSE_AGREEMENT
```

### CITATION
```
CITATION.md
CITATION
CITATION.cff             # Citation File Format (recommended)
REFERENCES.md
REFERENCES
```

### ROADMAP
```
ROADMAP.md
ROADMAP
TODO.md
TODO
PLAN.md
PLAN
FUTURE.md
FUTURE
```

### ADOPTERS
```
ADOPTERS.md
ADOPTERS
USERS.md
USERS
SHOWCASE.md
SHOWCASE
PROJECTS.md
PROJECTS
```

### MANIFESTO
```
MANIFESTO.md
MANIFESTO
VISION.md
VISION
PHILOSOPHY.md
PHILOSOPHY
PRINCIPLES.md
PRINCIPLES
```

### INSTALL
```
INSTALL.md
INSTALL
INSTALLATION.md
INSTALLATION
```

### BUILD
```
BUILD.md
BUILD
BUILDING.md
BUILDING
COMPILE.md
COMPILE
MAKE.md
```

### DEPENDENCIES
```
DEPENDENCIES.md
DEPENDENCIES
REQUIREMENTS.md
REQUIREMENTS
PREREQUISITES.md
PREREQUISITES
```

**Note:** For language-specific dependencies, use standard files:
- Python: `requirements.txt`, `pyproject.toml`
- Node.js: `package.json`
- Rust: `Cargo.toml`
- Go: `go.mod`
- Ruby: `Gemfile`

### GUIDE
```
GUIDE.md
GUIDE
TUTORIAL.md
TUTORIAL
QUICKSTART.md
QUICKSTART
```

### FAQ
```
FAQ.md
FAQ
```

### EXAMPLES
```
EXAMPLES.md
EXAMPLES
examples/         # Directory (lowercase)
```

### ARCHITECTURE
```
ARCHITECTURE.md
ARCHITECTURE
DESIGN.md
DESIGN
```

### API
```
API.md
API
API_REFERENCE.md
API_REFERENCE
openapi.yaml      # For REST APIs
swagger.json      # For REST APIs
```

### MIGRATION
```
MIGRATION.md
MIGRATION
UPGRADING.md
UPGRADING
```

### VERSION
```
VERSION
VERSION.txt
.version
```

### FUNDING
```
FUNDING.md
FUNDING
FUNDING.yml       # GitHub-specific, in .github/
SPONSORS.md
SPONSORS
```

### CODEOWNERS
```
CODEOWNERS
.github/CODEOWNERS
docs/CODEOWNERS
```

## Configuration Files

These have specific formats and are typically lowercase:

```
.gitignore
.gitkeep / .keep
.gitattributes
.gitmodules
.dockerignore
.editorconfig
```

## Best Practices

1. **Be consistent** - Pick one variant and stick to it
2. **UPPER_CASE for documentation** - It's the standard
3. **Use .md for new files** - Most widely supported
4. **Follow platform conventions** - GitHub recognizes specific names
5. **Document unusual choices** - If using non-standard names, explain why
6. **Don't use both variants** - Choose one (README.md OR readme.md, not both)

## Platform Recognition

Some platforms (GitHub, GitLab, Bitbucket) recognize specific filenames:

**GitHub:**
- `SECURITY.md` - Adds Security tab
- `FUNDING.yml` - Adds Sponsor button
- `CODEOWNERS` - Auto-assigns reviewers
- `CITATION.cff` - Citation widget
- Issue/PR templates in `.github/`

**Best Practice:** Use recognized names for better platform integration.
