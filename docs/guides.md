# Installation & Build Guides

Documentation for installing, building, and using your project. Essential for user adoption.

## INSTALL

Installation instructions for end users.

### Required Contents
- System requirements (OS, hardware, dependencies)
- Installation methods (package managers, binary downloads, source builds)
- Platform-specific instructions for different operating systems
- Post-installation verification steps
- Troubleshooting guide for common installation issues
- Uninstallation instructions
- Upgrade procedures from previous versions

### When to Separate from README
- Complex multi-step installation process
- Multiple installation methods available
- Platform-specific instructions are lengthy
- README becomes too long with installation details

### Naming Variants
- `INSTALL.md`
- `INSTALL`
- `INSTALLATION.md`
- `INSTALLATION`

## BUILD

Build instructions for developers compiling from source.

### Required Contents
- Build dependencies list with version requirements
- Required build tools (compilers, build systems)
- Step-by-step build process
- Build configuration options and flags
- Platform-specific build notes and requirements
- Test execution procedures after building
- Debug vs release build instructions
- Cross-compilation instructions (if applicable)
- Build troubleshooting guide

### Naming Variants
- `BUILD.md`
- `BUILD`
- `BUILDING.md`
- `BUILDING`
- `COMPILE.md`
- `COMPILE`
- `MAKE.md`

### Distinction from INSTALL
- BUILD is for developers building from source
- INSTALL is for users installing pre-built packages

## DEPENDENCIES

List of project dependencies and their purposes.

### Required Contents
- Runtime dependencies with version requirements
- Build-time dependencies
- Optional dependencies and their purposes
- System library requirements
- Justification for each major dependency
- Dependency update policy
- Known compatibility issues

### Language-Specific Alternatives
Many languages have standardized dependency files that should be preferred:
- Python: `requirements.txt`, `Pipfile`, `pyproject.toml`, `setup.py`
- Node.js: `package.json`
- Rust: `Cargo.toml`
- Go: `go.mod`
- Ruby: `Gemfile`
- PHP: `composer.json`

### When to Use DEPENDENCIES.md
- Multi-language projects without single dependency system
- System-level dependencies not managed by language tools
- Explaining rationale for dependency choices
- Complex dependency relationships requiring documentation
- Dependencies that cannot be expressed in standard files

### Naming Variants
- `DEPENDENCIES.md`
- `DEPENDENCIES`
- `REQUIREMENTS.md`
- `REQUIREMENTS`
- `PREREQUISITES.md`
- `PREREQUISITES`

## GUIDE

Comprehensive usage guide or tutorial.

### Required Contents
- Getting started tutorial
- Common use cases with explanations
- Advanced features documentation
- Configuration options
- Best practices
- Performance tuning guide
- Migration guides from similar tools
- Troubleshooting section

### When to Use
- Complex projects needing detailed walkthroughs
- Alternative to separate `docs/` directory for smaller projects
- Quick start tutorials
- Not recommended when full `docs/` directory exists

### Naming Variants
- `GUIDE.md`
- `GUIDE`
- `TUTORIAL.md`
- `TUTORIAL`
- `QUICKSTART.md`
- `QUICKSTART`

### Alternative: docs/ Directory
For larger projects, create structured documentation directory:
- `docs/getting-started.md`
- `docs/installation.md`
- `docs/configuration.md`
- `docs/api-reference.md`
- `docs/tutorials/`
- `docs/examples/`

## Best Practices

1. **INSTALL for users, BUILD for developers** - Clear separation of concerns
2. **Use language-standard dependency files** - Don't create custom systems
3. **Link from README** - Make guides easily discoverable
4. **Keep instructions current** - Test them regularly on clean systems
5. **Include verification steps** - Help users confirm successful completion
6. **Platform-specific sections** - Use clear headings and organization
7. **One-line install preferred** - Simplify when possible (package managers, installers)
8. **Version compatibility** - Document which versions work together
9. **Offline installation** - Document procedures for air-gapped environments
10. **Update regularly** - Instructions become outdated quickly
