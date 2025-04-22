# ⚙️ Personal Setup & Configuration Files

This repository contains my personal configuration files used to standardise and streamline development across different environments. It’s a collection of tools and settings that help me write clean, consistent, and well-formatted code from project to project.

---

## 📂 What's Inside

| File                          | Purpose                                                                |
|------------------------------|------------------------------------------------------------------------|
| `.editorconfig`              | Ensures consistent coding styles across different editors and IDEs     |
| `.gitconfig`                 | Personal Git settings (e.g., aliases, user info, default behaviour)     |
| `.pre-commit-config.yaml`    | Hooks for code quality checks before commits (e.g., Black, isort)       |
| `pyproject.toml`             | Python project configuration (e.g., formatter, linter, tool settings)   |
| `settings.json`              | VS Code-specific settings for editor preferences and extensions         |
| `README.md`                  | You're reading it!                                                     |

---

## 🛠️ How I Use This Repo

This setup is meant to be **modular and portable** — I can clone or symlink specific files into new projects or dev machines to instantly apply my preferred settings.

### 🔄 Example Usage

```bash
# Clone into a hidden folder in home
git clone https://github.com/jswalker-data/Setup ~/.dotfiles

# Symlink gitconfig
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig
```

Or selectively copy configs into your project root for consistency.

---

## 🧹 Pre-commit Hooks

This repo uses [pre-commit](https://pre-commit.com/) to enforce code quality and consistency automatically before each commit or push.

### 🔧 Tools Included

- **[Ruff](https://github.com/astral-sh/ruff)** – Lightning-fast Python linter & formatter (with `--fix` enabled)
- **Trailing whitespace removal**
- **End-of-file fixer**
- **YAML, JSON, TOML, and XML checkers**
- **Merge conflict & symlink detection**
- **Private key detector**
- **Auto-format JSON files** with 2-space indent and no key sorting
- **Auto-update hook** to keep everything up to date

### ⚙️ Setup Instructions

To get started:

```bash
pip install pre-commit
pre-commit install
```

Then you can manually run hooks with:

```bash
pre-commit run --all-files
```

The hooks are triggered on both `pre-commit` and `pre-push` stages for maximum protection against bad code slipping in.

---

## 🧪 Compatible With

- ✅ Python development environments
- ✅ Git workflows
- ✅ VS Code (via `settings.json`)
- ✅ Most modern editors (via `.editorconfig`)

---

## 🌱 Why I Use This

Having a shared setup:
- Ensures **code consistency** across projects and team members
- Reduces onboarding/setup time on new machines
- Makes **pre-commit and formatting** seamless and automatic

---

Feel free to fork, clone, or cherry-pick any part of this setup if it’s helpful to you!



