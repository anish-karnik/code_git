# 🚀 UGIT - A Minimal Git Implementation

![UGIT Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQiwMRyK4rv7q_Ocr4uQk_3fD4PAyqr_6GbxQ&s)  

> A lightweight, educational version-control system built in Python 🐍.

UGIT is a minimalistic version control system that replicates Git's core functionalities. Whether you're learning how Git works under the hood or need a simple tool for tracking changes, UGIT provides a straightforward experience.

---

## 📖 Table of Contents

- [📦 Installation](#-installation)
- [⚡ Quick Start](#-quick-start)
- [✨ Features](#-features)
- [🛠️ Commands](#️-commands)
- [🔧 Configuration](#-configuration)
- [📜 Dependencies](#-dependencies)
- [📌 Examples](#-examples)
- [❓ Troubleshooting](#-troubleshooting)
- [👥 Contributors](#-contributors)
- [📜 License](#-license)

---

## 📦 Installation

UGIT requires Python 3.x. You can install it using `pip`:

```sh
pip install .
```

Alternatively, you can clone the repository and install manually:

```sh
git clone https://github.com/your-repo/ugit.git
cd ugit
python setup.py install
```

After installation, the `ugit` command becomes available globally:

```sh
ugit <command> [options]
```

---

## ⚡ Quick Start

### 1️⃣ Initialize a Repository
```sh
ugit init
```

### 2️⃣ Add Files & Commit
```sh
ugit add myfile.txt
ugit commit -m "Initial commit"
```

### 3️⃣ View Commit Log
```sh
ugit log
```

### 4️⃣ Push Changes
```sh
ugit push origin main
```

---

## ✨ Features

✔️ Create and manage repositories  
✔️ Stage and commit files  
✔️ View commit logs and history  
✔️ Diff changes between files  
✔️ Merge branches  
✔️ Push and fetch from remote repositories  
✔️ Reset changes and roll back  
✔️ Compare trees for efficient merging  
✔️ **Command-line interface (CLI) support**  

---

## 🛠️ Commands

| Command                     | Description |
|-----------------------------|-------------|
| `init`                      | Initialize a repository |
| `status`                    | Show repository status |
| `log`                       | Display commit history |
| `show`                      | Show commit details |
| `add <files>`               | Stage files for commit |
| `commit -m "<message>"`     | Commit staged changes |
| `checkout <commit>`         | Switch branches or restore files |
| `branch <name>`             | Create a new branch |
| `merge <commit>`            | Merge branches |
| `reset <commit>`            | Reset HEAD to a specific commit |
| `diff [--cached] [commit]`  | Show differences between commits |
| `fetch <remote>`            | Fetch updates from a remote repository |
| `push <remote> <branch>`    | Push changes to a remote repository |

---

## 🔧 Configuration

UGIT stores its data in the `.ugit` directory inside the repository. Configuration is managed within `data.py`, handling:

- Object storage
- Reference management
- Indexing

---

## 📜 Dependencies

UGIT is implemented using Python's standard libraries:

- `argparse` → CLI parsing  
- `os`, `shutil` → File handling  
- `hashlib` → Object hashing  
- `subprocess` → Diff and merge execution  

**No external dependencies!** 🎉

---

## 📌 Examples

### 📍 View File Content
```sh
ugit cat-file <object-id>
```

### 📍 Create a Branch and Switch
```sh
ugit branch feature-x
ugit checkout feature-x
```

### 📍 Merge Changes
```sh
ugit merge <commit>
```

### 📍 Fetch and Push to Remote
```sh
ugit fetch origin
ugit push origin main
```

---

## ❓ Troubleshooting

🔹 **Command not found?** Ensure UGIT is installed via `pip install .` or `python setup.py install`.  
🔹 **Merge conflicts?** Use `diff` before merging to preview changes.  
🔹 **Repository not initialized?** Run `init` before other commands.  

For detailed help, use:
```sh
ugit --help
```

---

## 👥 Contributors

| Name         | GitHub Profile |
|-------------|---------------|
| **Anish Karnik** | [GitHub](https://github.com/anish-karnik) |

Want to contribute? Open an issue or create a pull request!

---

## 📜 License

📄 This project is licensed under the **MIT License**.
