# Contributing to PouchVerse

Thank you for your interest in improving PouchVerse's documentation and translations!

> 简体中文贡献指南请见 [CONTRIBUTING.zh-Hans.md](CONTRIBUTING.zh-Hans.md)。

---

## What You Can Contribute

This is the **public release repository** for PouchVerse — it contains documentation, translations, legal documents, the user manual, and app store screenshots. Contributions in the following areas are welcome:

- **Documentation fixes** — typos, broken links, formatting issues
- **Translation improvements** — corrections or natural-sounding rephrasing
- **New translations** — if you'd like to add a language not yet supported
- **Screenshot updates** — if you have access to newer or higher-quality assets

> **App source code** is not hosted here. For feature requests or app bugs, please [open an Issue](https://github.com/ejiandan/PouchVerse-release/issues/new/choose).

---

## Getting Started

1. **Fork** this repository
2. **Clone** your fork locally
3. Create a new **branch** for your change:
   ```
   git checkout -b fix/typo-in-readme-es
   ```
4. Make your changes
5. **Commit** with a clear message (see below)
6. **Push** to your fork and open a **Pull Request**

---

## Commit Message Convention

We follow a lightweight convention:

```
<type>(<scope>): <short description>
```

| Type     | When to use                                      |
|----------|--------------------------------------------------|
| `fix`    | Fixing a typo, broken link, or incorrect info    |
| `feat`   | Adding new content (e.g. a new translation file) |
| `chore`  | Asset updates, metadata changes                  |
| `docs`   | Improving structure or clarity of documentation  |

**Examples:**
```
fix(ja): correct mistranslated section in Quick-Start.ja.md
feat(fr): add French translation for README
chore: update iPhone screenshots for iOS 18
```

---

## Translation Guidelines

- Translate **meaning**, not word-for-word
- Use natural, native phrasing for the target language
- Keep **technical terms** (e.g. SHA-256, LAN, Face ID) untranslated unless a widely accepted local equivalent exists
- Preserve all **Markdown formatting** (bold, links, headings, tables)
- Match the **same heading structure** as the English source (`README.md`)

### Supported Languages

| Language              | File suffix    |
|-----------------------|----------------|
| English               | (no suffix)    |
| Simplified Chinese    | `.zh-Hans`     |
| Traditional Chinese   | `.zh-Hant`     |
| Japanese              | `.ja`          |
| Korean                | `.ko`          |
| Spanish               | `.es`          |

---

## Pull Request Checklist

Before submitting a PR, please confirm:

- [ ] Changes are limited to the described scope
- [ ] Spelling and grammar have been checked
- [ ] All links in changed files are valid
- [ ] Markdown renders correctly (use the GitHub preview)
- [ ] For translations: meaning matches the English source

---

## Questions?

Open a [Discussion](https://github.com/ejiandan/PouchVerse-release/discussions) for general questions, or an [Issue](https://github.com/ejiandan/PouchVerse-release/issues) for specific problems.
