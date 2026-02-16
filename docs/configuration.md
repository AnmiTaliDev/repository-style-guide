# Configuration Files

Configuration files for version control, containers, and development tools.

## Git Configuration Files

### .gitignore

Specifies intentionally untracked files that Git should ignore.

**Purpose:**
- Exclude build artifacts and compiled code
- Ignore IDE and editor-specific files
- Keep secrets and credentials out of repository
- Reduce repository size and clutter
- Prevent accidental commits of temporary files

**Required Content Categories:**
- Build outputs (binaries, compiled files, distribution packages)
- Dependencies directories (node_modules, vendor, etc.)
- IDE and editor files (.vscode, .idea, *.swp)
- Operating system files (.DS_Store, Thumbs.db)
- Secrets and credentials (.env, *.key, *.pem)
- Log files and temporary files
- Cache directories

**Best Practices:**
- Use gitignore.io for language and framework-specific templates
- Include language-specific ignores
- Add project-specific ignores
- Document unusual ignore patterns
- Keep organized with comments

### .gitkeep

**IMPORTANT:** Not an official Git file - this is a community convention.

**Purpose:**
- Git does not track empty directories
- `.gitkeep` forces Git to track empty directories by being a tracked file inside them
- Alternative name: `.keep` (also not official, same purpose)

**When to Use:**
- Directory structure must exist for application to function
- Directories for log files, uploads, cache that start empty
- Build systems expecting specific directory structure
- Data directories that will be populated at runtime

**Alternatives:**
- `.keep` (shorter name, same convention)
- Any tracked file (README.md explaining the directory)
- Some projects use empty `.gitignore` files

### .gitattributes

Controls how Git handles line endings, diffs, and merges.

**Purpose:**
- Normalize line endings across different operating systems
- Control diff behavior for specific file types
- Mark files as binary or text
- Configure merge strategies
- Control export and archive behavior
- Mark generated files for GitHub Linguist

**Common Use Cases:**
- Line ending normalization (LF vs CRLF)
- Force specific line endings for scripts
- Mark binary files explicitly
- Define custom diff algorithms for specific file types
- Identify generated files
- Control whitespace handling

**When to Include:**
- Cross-platform projects (Windows, Mac, Linux)
- Projects with binary files
- When line endings are critical (shell scripts, config files)
- Projects with generated files in repository
- Multi-language projects

### .gitmodules

Configuration file for Git submodules.

**Purpose:**
- Define external repositories included as subdirectories
- Specify submodule URLs and paths
- Track specific commits of external dependencies

**Content Structure:**
- Submodule path within the repository
- Remote URL of the submodule repository
- Optional: specific branch to track

**Best Practices:**
- Place submodules in `3rd/` directory (recommended convention)
- Alternative directory names: `vendor/`, `external/`, `deps/`
- Document why each submodule is used
- Pin to specific commits or tags for stability
- Consider alternatives (package managers) before using submodules

**Common Directory Structures:**
- `3rd/` - Third-party code (recommended)
- `vendor/` - Alternative common name
- `external/` - Alternative name
- `deps/` - Alternative name for dependencies

## Docker Configuration

### .dockerignore

Similar to `.gitignore` but for Docker build context.

**Purpose:**
- Reduce Docker build context size
- Faster Docker builds
- Avoid copying secrets into Docker images
- Reduce image size
- Prevent unnecessary cache invalidation

**Required Content Categories:**
- Version control directories (.git, .gitignore)
- Docker-related files (Dockerfile, docker-compose.yml, .dockerignore)
- Documentation (README.md, CHANGELOG.md, docs/)
- Development tools (.vscode/, .idea/)
- Log files
- Dependencies if installed in Dockerfile
- Build outputs if built in Dockerfile
- Test files and test data
- CI/CD configuration files

**When to Include:**
- Every project with a Dockerfile
- Essential for production builds
- Even simple projects benefit from it

## Editor Configuration

### .editorconfig

Ensures consistent coding style across different editors and IDEs.

**Purpose:**
- Define consistent formatting rules
- Works across multiple editors
- Reduces style inconsistencies in contributions
- Eliminates formatting arguments
- Automatic style enforcement

**Supported Properties:**
- `indent_style` - tabs or spaces
- `indent_size` - number of spaces or tab width
- `end_of_line` - lf, crlf, or cr
- `charset` - file encoding (utf-8, etc.)
- `trim_trailing_whitespace` - true/false
- `insert_final_newline` - true/false
- `max_line_length` - character limit

**File Pattern Matching:**
- Global rules for all files
- Language-specific rules
- File extension specific rules
- Filename specific rules (Makefile, etc.)

**Editor Support:**
Works in VSCode, IntelliJ IDEA, Vim, Emacs, Sublime Text, Atom, and many others.

**When to Include:**
- Highly recommended for multi-developer projects
- Essential for open source projects accepting contributions
- Any project expecting external contributors
- Teams with mixed editor preferences

## Best Practices

1. **Always include .gitignore** - Even for small projects
2. **Use .gitkeep wisely** - Only for directories that must exist empty
3. **Use .gitattributes** - Prevents cross-platform line ending issues
4. **Submodules in 3rd/** - Clear, conventional organization
5. **Always use .dockerignore** - With every Dockerfile
6. **Use .editorconfig** - For consistent formatting
7. **Document conventions** - If using non-standard locations or patterns
8. **Keep updated** - Review and update as project evolves
9. **Test configurations** - Verify they work as intended
10. **Use templates** - Start with established templates for your tech stack

## Debian Packaging (for CI/CD)

### debian/ Directory

For projects that want to be packaged as Debian/Ubuntu packages.

**Purpose:**
- Native Debian/Ubuntu package creation
- Integration with apt package manager
- Professional Linux distribution

**Required Files:**
- `changelog` - Version history in Debian format
- `control` - Package metadata and dependencies
- `copyright` - Licensing information
- `rules` - Build instructions
- `compat` - Debhelper compatibility level
- `source/format` - Source package format specification

**When to Include:**
- Projects targeting Debian/Ubuntu distributions
- Professional Linux software
- Software intended for official repositories
- Enterprise Linux deployments
