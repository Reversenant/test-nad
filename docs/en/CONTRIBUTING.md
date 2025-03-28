# 🤝 Contributing Guide

Thank you for your interest in the project! Here's how you can contribute:

## 🚀 Getting Started

1. Fork the repository
2. Create a new branch:
```
git checkout -b feature/your_feature
```
3. Make all necessary changes
4. Be sure to test your code
5. Create a Pull Request to `main` or `dev` (confirm if unsure)

## ✅ What We Appreciate

- Improving documentation
- Reporting issues
- New features (ideally after discussion)
- Adding new tests for existing functionality

## 🧹 Code Style

- Follow formatting and style guidelines (eslint/black/prettier)
- Try to write meaningful commit messages:
```
feature: Added support for X
fix: Fixed bug Y
docs: Updated documentation
```

## 🌐 Want to Help with Translation?

We aim to make the project accessible to as many people as possible. If you'd like to help translate into another language — it's very welcome!

📄 Available translations:
- 🇺🇸 English (default)
- 🇷🇺 Russian (in progress)
- 🌐 Your language? Help us add it!

Create a corresponding issue.

## 🛠 Best Practices

- Use stable dependency versions listed in `package.json` / `requirements.txt` / `pyproject.toml`
- Follow the project's coding style (e.g., via `eslint`, `black`, `prettier`, etc.)
- Write readable and self-documenting code
- Try to cover new functionality with tests
- Before creating an issue — check if a similar one already exists
- Create feature branches and submit pull requests with clear descriptions

![image](../assets/pic_left.svg)

# ✍️ Developer Certificate of Origin (DCO)

Thank you for your contribution! To ensure transparency and legal clarity in the project, we use the **Developer Certificate of Origin (DCO)**.

## 📜 What is DCO?

The DCO is a simple statement that you have the right to submit the code you’re contributing and that you agree to the project’s license. This is especially important for open source projects.

Full DCO text: [https://developercertificate.org](https://developercertificate.org)

## ✅ What do you need to do?

**Every commit must be signed.** You can do this by adding the `-s` flag when creating a commit:

```bash
git commit -s -m "fix: fixed error handling"
```

Example of a commit signature:

```
Signed-off-by: John Doe <john@example.com>
```

## 🛠 Configure your name and email

Make sure Git is configured with your name and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

## 🔁 How to re-sign commits

If you forgot to sign a commit:

### One commit

```bash
git commit --amend -s
git push --force
```

### Multiple commits

```bash
git rebase -i HEAD~N  # Replace N with the number of recent commits
```

Change `pick` to `edit` for the commits you want to sign, and for each:

```bash
git commit --amend -s
git rebase --continue
```

After finishing the rebase:

```bash
git push --force
```

> ⚠️ Warning: use `--force` with caution, especially when working in a team.