# Соглашения по именованию и синонимы файлов

Руководства по именованию файлов, форматам и принятым синонимам в профессиональных репозиториях.

## Общие соглашения

### Стиль регистра
**Стандарт: UPPER_CASE**

Стандартные документационные файлы должны использовать UPPER_CASE (README.md, LICENSE, CONTRIBUTING.md, CODE_OF_CONDUCT.md). Нижний регистр приемлем, но не является стандартом (readme.md приемлемо, но не стандарт). Смешанный регистр непоследователен (избегайте Readme.md).

**Исключения:**
- `docs/` — Обычно в нижнем регистре
- `examples/` — Обычно в нижнем регистре
- Языко-специфичные файлы: `package.json`, `requirements.txt` и т.д.
- Конфигурационные файлы: `.gitignore`, `.editorconfig` и т.д.

### Форматы файлов

**Рекомендуется:** Используйте форматы разметки, не простой текст

Предпочтительные форматы: `.md` (Markdown) — наиболее распространённый; `.rst` (reStructuredText) — распространён в Python; `.tex` (LaTeX) — академические проекты; `.adoc` (AsciiDoc) — техническая документация.

Избегайте: `.txt` и файлов без расширения (кроме LICENSE, который может быть без расширения).

### Подчёркивания vs дефисы
- **Стандарт:** Подчёркивания (`_`)
- Примеры: `CODE_OF_CONDUCT.md`, `PULL_REQUEST_TEMPLATE.md`
- Дефисы приемлемы для форматов: `LICENSE-GPL-3.0`

## Полный справочник синонимов

### README
- `README.md`
- `README`
- `README.rst`
- `README.tex`
- `readme.md`
- `ReadMe.md`

### LICENSE
- `LICENSE`
- `LICENSE.md`
- `LICENSE.txt`
- `LICENSE-<название-лицензии>` (например, LICENSE-GPL-3.0)
- `LICENSE-<название-лицензии>.md` (например, LICENSE-MIT.md)
- `LICENCE` (британское написание)
- `LICENCE.md`
- `COPYING`
- `COPYING.md`

### CHANGELOG
- `CHANGELOG.md`
- `CHANGELOG`
- `HISTORY.md`
- `HISTORY`
- `NEWS.md`
- `NEWS`
- `RELEASES.md`
- `RELEASES`
- `CHANGES.md`
- `CHANGES`

### CONTRIBUTING
- `CONTRIBUTING.md`
- `CONTRIBUTING`
- `HACKING.md`
- `HACKING`
- `DEVELOPMENT.md`
- `DEVELOPMENT`

### CODE_OF_CONDUCT
- `CODE_OF_CONDUCT.md`
- `CODE_OF_CONDUCT`
- `CONDUCT.md`
- `CONDUCT`
- `CoC.md`
- `CoC`

### SUPPORT
- `SUPPORT.md`
- `SUPPORT`
- `HELP.md`
- `HELP`
- `CONTACT.md`
- `CONTACT`
- `TROUBLESHOOTING.md`
- `TROUBLESHOOTING`

### GOVERNANCE
- `GOVERNANCE.md`
- `GOVERNANCE`
- `CHARTER.md`
- `CHARTER`
- `DECISIONS.md`
- `DECISIONS`

### AUTHORS / CONTRIBUTORS / MAINTAINERS
- `AUTHORS.md`
- `AUTHORS`
- `CONTRIBUTORS.md`
- `CONTRIBUTORS`
- `MAINTAINERS.md`
- `MAINTAINERS`
- `CREDITS.md`
- `CREDITS`
- `OWNERS`
- `THANKS.md`
- `THANKS`
- `MEMBERS.md`
- `MEMBERS`
- `CORE_TEAM.md`
- `CORE_TEAM`
- `STEWARDS.md`
- `STEWARDS`

### ACKNOWLEDGMENTS
- `ACKNOWLEDGMENTS.md`
- `ACKNOWLEDGMENTS`
- `ACKNOWLEDGEMENTS.md` (британское написание)
- `ACKNOWLEDGEMENTS`
- `ATTRIBUTIONS.md`
- `ATTRIBUTIONS`
- `THANKS.md`
- `THANKS`

### SECURITY
- `SECURITY.md`
- `SECURITY`
- `VULNERABILITIES.md`
- `VULNERABILITIES`
- `SECURITY_POLICY.md`
- `POLICY.md`

### PRIVACY
- `PRIVACY.md`
- `PRIVACY`
- `PRIVACY_POLICY.md`
- `DATA_USAGE.md`
- `DATA_USAGE`
- `GDPR.md`
- `GDPR`

### TRADEMARK
- `TRADEMARK.md`
- `TRADEMARK`
- `BRAND_GUIDELINES.md`
- `BRAND_GUIDELINES`
- `LOGO.md`
- `LOGO`
- `BRANDING.md`
- `BRANDING`

### NOTICE
- `NOTICE`
- `NOTICE.md`
- `LEGAL.md`
- `LEGAL`
- `DISCLAIMER.md`
- `DISCLAIMER`

### DCO
- `DCO`
- `DCO.md`
- `DEVELOPER_CERTIFICATE.md`
- `DEVELOPER_CERTIFICATE_OF_ORIGIN.md`

### CLA
- `CLA.md`
- `CLA`
- `CONTRIBUTOR_LICENSE_AGREEMENT.md`
- `CONTRIBUTOR_LICENSE_AGREEMENT`

### CITATION
- `CITATION.md`
- `CITATION`
- `CITATION.cff` (Citation File Format — рекомендуется)
- `REFERENCES.md`
- `REFERENCES`

### ROADMAP
- `ROADMAP.md`
- `ROADMAP`
- `TODO.md`
- `TODO`
- `PLAN.md`
- `PLAN`
- `FUTURE.md`
- `FUTURE`

### ADOPTERS
- `ADOPTERS.md`
- `ADOPTERS`
- `USERS.md`
- `USERS`
- `SHOWCASE.md`
- `SHOWCASE`
- `PROJECTS.md`
- `PROJECTS`

### MANIFESTO
- `MANIFESTO.md`
- `MANIFESTO`
- `VISION.md`
- `VISION`
- `PHILOSOPHY.md`
- `PHILOSOPHY`
- `PRINCIPLES.md`
- `PRINCIPLES`

### INSTALL
- `INSTALL.md`
- `INSTALL`
- `INSTALLATION.md`
- `INSTALLATION`

### BUILD
- `BUILD.md`
- `BUILD`
- `BUILDING.md`
- `BUILDING`
- `COMPILE.md`
- `COMPILE`
- `MAKE.md`

### DEPENDENCIES
- `DEPENDENCIES.md`
- `DEPENDENCIES`
- `REQUIREMENTS.md`
- `REQUIREMENTS`
- `PREREQUISITES.md`
- `PREREQUISITES`

**Примечание:** Для языко-специфичных зависимостей используйте стандартные файлы:
- Python: `requirements.txt`, `pyproject.toml`
- Node.js: `package.json`
- Rust: `Cargo.toml`
- Go: `go.mod`
- Ruby: `Gemfile`

### GUIDE
- `GUIDE.md`
- `GUIDE`
- `TUTORIAL.md`
- `TUTORIAL`
- `QUICKSTART.md`
- `QUICKSTART`

### FAQ
- `FAQ.md`
- `FAQ`

### EXAMPLES
- `EXAMPLES.md`
- `EXAMPLES`
- `examples/` (директория, в нижнем регистре)

### ARCHITECTURE
- `ARCHITECTURE.md`
- `ARCHITECTURE`
- `DESIGN.md`
- `DESIGN`

### API
- `API.md`
- `API`
- `API_REFERENCE.md`
- `API_REFERENCE`
- `openapi.yaml` (для REST API)
- `swagger.json` (для REST API)

### MIGRATION
- `MIGRATION.md`
- `MIGRATION`
- `UPGRADING.md`
- `UPGRADING`

### VERSION
- `VERSION`
- `VERSION.txt`
- `.version`

### FUNDING
- `FUNDING.md`
- `FUNDING`
- `FUNDING.yml` (GitHub-специфичный, в .github/)
- `SPONSORS.md`
- `SPONSORS`

### CODEOWNERS
- `CODEOWNERS`
- `.github/CODEOWNERS`
- `docs/CODEOWNERS`

## Конфигурационные файлы

Эти файлы имеют специфические форматы и обычно в нижнем регистре:

- `.gitignore`
- `.gitkeep` / `.keep`
- `.gitattributes`
- `.gitmodules`
- `.dockerignore`
- `.editorconfig`

## Лучшие практики

1. **Будьте последовательны** — Выберите один вариант и придерживайтесь его
2. **UPPER_CASE для документации** — Это стандарт
3. **Используйте .md для новых файлов** — Самая широкая поддержка
4. **Следуйте соглашениям платформы** — GitHub распознаёт специфичные имена
5. **Документируйте необычный выбор** — Если используете нестандартные имена, объясните почему
6. **Не используйте оба варианта** — Выберите один (README.md ИЛИ readme.md, не оба)

## Распознавание платформами

Некоторые платформы (GitHub, GitLab, Bitbucket) распознают специфичные имена файлов:

**GitHub:**
- `SECURITY.md` — Добавляет вкладку Security
- `FUNDING.yml` — Добавляет кнопку Sponsor
- `CODEOWNERS` — Автоназначение ревьюеров
- `CITATION.cff` — Виджет цитирования
- Шаблоны Issue/PR в `.github/`

**Лучшая практика:** Используйте распознаваемые имена для лучшей интеграции с платформой.
