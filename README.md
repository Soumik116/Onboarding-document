# Welcome to Git and Github at ChaiCode Cohort!

Learning by reading documentation is very important, even essential, as a developer. As a developer, you will have to read a lot of documentation to learn about new technologies coming into the market every day. So, it’s good to build a habit of reading documentation. We will learn Git and GitHub by reading documentation.

## Getting Started with Git and GitHub

If you're new to Git and GitHub, don't worry! We'll start from the basics and guide you through. By the end of this onboarding guide, you'll have a solid understanding of how to use Git, GitHub, and their essential features for collaborating on projects.

---

### What Are Git and GitHub?

- **Git**: A **Version Control System (VCS)** that helps you track changes in your code. Think of it as a checkpoint system for your code—every time you make a commit, Git saves your code's history, allowing you to access it later.
- **GitHub**: An **online platform** that provides a beautiful user interface for Git. It makes collaboration easy by enabling teams to work on projects from anywhere in the [world](http://world.it). It is an essential tool for team collaboration.

---

### Step 1: Installing Git

1. Open any browser and search for **Git download**.
2. Download Git for your specific operating system (Windows, macOS, or Linux).

![Git Download](path/to/git-download.png)

3. Install Git on your system.
4. During installation, you'll also get **Git Bash**, a terminal ideal for learning Git commands.

> **Pro Tip:** While you can use other terminals (like VS Code's terminal), some Git commands work best on Git Bash.

5. Open [GitHub](http://github.com) and create an account.

![GitHub Signup](path/to/github-signup.png)

---

### Step 2: Setting Up Git

After installation, follow these steps to configure Git:

1. Open Git Bash.
2. Run the following commands to set your username and email (used for commit tracking):

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```

3. To verify the configuration, use:

   ```bash
   git config --list
   ```

---

### Step 3: Cloning a Repository

1. Open the GitHub repository you want to copy, click on the **Code** button, and copy the repository link.
2. Create a folder on your computer to store the repository.
3. Open Git Bash, navigate to the folder using:

   ```bash
   cd <folder-directory>
   ```

4. Clone the repository using:

   ```bash
   git clone "repository-link"
   ```

5. Navigate into the cloned repository:

   ```bash
   cd <repository-folder-name>
   ```

---

### Step 4: Basic Git Commands

Here are some essential Git commands you'll use frequently:

| **Command**              | **Description**                                                             |
|---------------------------|-----------------------------------------------------------------------------|
| `git init`               | Initializes a new Git repository in the current directory.                 |
| `git status`             | Shows the status of your repository (e.g., changes, untracked files).      |
| `git add <file>`         | Adds specific files to the staging area.                                   |
| `git add .`              | Adds all changes in the directory to the staging area.                     |
| `git commit -m "message"`| Saves changes to the repository with a descriptive message.                |
| `git log`                | Displays the commit history.                                               |
| `git diff`               | Shows changes between commits, the working directory, and the staging area.|
| `git clone <url>`        | Clones an existing repository from GitHub to your local machine.           |
| `git push`               | Pushes local changes to the remote repository.                             |
| `git pull`               | Fetches and merges changes from the remote repository.                     |

---

### Step 5: Getting Started with GitHub

1. **Sign Up:** Create an account at [GitHub](https://github.com/).
2. **Create a Repository:**
   - Click on "New Repository" and give it a name.
   - Choose whether it will be public or private.
3. **Connect Git to GitHub:**
   - Copy the repository's URL.
   - In your terminal, run:

     ```bash
     git remote add origin <repository-url>
     git push -u origin main
     ```

---

### Creating a Pull Request (PR)

1. Navigate to your GitHub repository.
2. Go to the **Pull Requests** tab and click on **New Pull Request**.
3. Select the branch you want to merge into the main branch.
4. Add a meaningful PR title and description.

#### Guidelines for Writing PR Descriptions:

- Clearly explain the purpose of the PR.
- Mention the key changes introduced.
- Include links to any relevant issues or tasks.

#### Requesting Code Reviews:

- Add reviewers to your PR to get feedback on your changes.
- Be open to constructive criticism and suggestions.

Leave some space here for screenshots.

---

### Best Practices for Using Git and GitHub

- **Write Clear Commit Messages:** Use descriptive messages that explain what your changes do. Example:

  ```
  Added user authentication feature
  ```

- **Commit Frequently:** Commit small, logical changes often to keep your project’s history clean.
- **Use Branches:** Create branches for new features or bug fixes. Example:

  ```bash
  git checkout -b feature/new-feature
  ```

- **Collaborate Effectively:** Use pull requests to review and discuss code changes with your team.
- **Resolve Conflicts:** When working with a team, learn how to resolve merge conflicts effectively.

---

### Commit Message Rules

Create rules for writing meaningful and standardized commit messages. For example:

- Use the present tense ("Add feature" not "Added feature").
- Capitalize the first letter.
- Keep the message short (50 characters or less).
- Use prefixes like `fix:`, `feat:`, `chore:`, `docs:` for categorization.

Example:

```bash
feat: Add tea selection feature
fix: Resolve login issue for tea enthusiasts
docs: Update README with chai varieties
```

---

### Creative Tip: Naming Your Branches

Use meaningful and consistent branch naming conventions:

- `feature/<feature-name>`: For new features.
- `bugfix/<issue-name>`: For fixing bugs.
- `hotfix/<critical-issue>`: For urgent fixes.

---

### Resources to Learn More

- [Official Git Documentation](https://git-scm.com/doc)
- [ChaiAurCode Docs](https://docs.chaicode.com/git-and-github/)

Welcome aboard, and happy coding! 🚀

