
Here's a **GitHub CLI Cheat Sheet** in English to help you quickly reference the most common commands and operations.

---

# **GitHub CLI (gh) Cheat Sheet**

### **1. Installation**
First, you need to install GitHub CLI if you haven't already:

**macOS:**
```bash
brew install gh
```

**Windows:**
```bash
winget install --id GitHub.cli
```

**Linux:**
```bash
sudo apt install gh
```

Once installed, you can verify the installation with:
```bash
gh --version
```

### **2. Authentication**
To authenticate the GitHub CLI with your account:

```bash
gh auth login
```
- You'll be prompted to choose between GitHub.com or GitHub Enterprise, and then a method of authentication (Browser, Token, etc.).
- To check if you are logged in, run:
  ```bash
  gh auth status
  ```

### **3. Basic GitHub CLI Commands**

#### **Repository Management**
- **Create a new repository:**
  ```bash
  gh repo create <repository-name> --public
  ```
  Options:
  - `--public`: Public repository.
  - `--private`: Private repository.

- **Clone a repository:**
  ```bash
  gh repo clone <owner/repo>
  ```

- **Fork a repository:**
  ```bash
  gh repo fork <owner/repo>
  ```

- **List your repositories:**
  ```bash
  gh repo list
  ```

- **View repository details:**
  ```bash
  gh repo view <owner/repo>
  ```
  Options:
  - `--web`: Open the repository in your web browser.

- **Delete a repository (Use carefully):**
  ```bash
  gh repo delete <owner/repo>
  ```

#### **Pull Requests (PR)**
- **Create a pull request:**
  ```bash
  gh pr create
  ```
  Options:
  - `--title <title>`: Title of the pull request.
  - `--body <body>`: Description for the pull request.

- **List pull requests:**
  ```bash
  gh pr list
  ```

- **View pull request details:**
  ```bash
  gh pr view <pr-number>
  ```

- **Merge a pull request:**
  ```bash
  gh pr merge <pr-number>
  ```
  Options:
  - `--squash`: Squash and merge.
  - `--rebase`: Rebase and merge.

- **Close a pull request without merging:**
  ```bash
  gh pr close <pr-number>
  ```

#### **Viewing in the Browser**
- **Open a repository in the browser:**
  ```bash
  gh repo view --web
  ```

- **Open an issue in the browser:**
  ```bash
  gh issue view <issue-number> --web
  ```

- **Open a pull request in the browser:**
  ```bash
  gh pr view <pr-number> --web
  ```


### **6. Help & Documentation**
- **Get help for any command:**
  ```bash
  gh <command> --help
  ```
  Example:
  ```bash
  gh pr --help
  ```

- **Full documentation:**  
  You can access the full GitHub CLI documentation at [GitHub CLI Docs](https://cli.github.com/manual/).

---
