# Welcome to Git and GitHub at ChaiCode Cohort!

Learning by reading documentation is very important and even essential as a developer. As a developer, you will have to read a lot of documentation to learn about new technologies coming to the market every day. So it’s good to build a habit of reading documentation. We will learn Git and GitHub by reading documentation.

## Getting Started with Git and GitHub

If you're new to Git and GitHub, don't worry! We'll start from the basics and guide you through. By the end of this onboarding guide, you'll have a solid understanding of how to use Git, GitHub, and their essential features for collaborating on projects.

---

### What Are Git and GitHub?

- **Git**: A **Version Control System (VCS)** that helps you track changes in your code. Think of it as a checkpoint system for your code—every time you make a commit, Git saves your code's history, allowing you to access it later.
- **GitHub**: An **online platform** that provides a beautiful user interface for Git. It makes collaboration easy by enabling teams to work on projects from anywhere in the world. It is an essential tool for team collaboration.

---

### Step 1: Installing Git

1. Open any browser and search for **Git download**.
2. Download Git for your specific operating system (Windows, macOS, or Linux).

![git download](https://github.com/user-attachments/assets/88f35455-82ad-4fad-a2f6-19813a19ea79)


3. Install Git on your system.
4. During installation, you'll also get **Git Bash**, a terminal ideal for learning Git commands.

> **Pro Tip**: While you can use other terminals (like VS Code's terminal), some Git commands work best on Git Bash.

5. Open [github.com](https://github.com) and create an account.

![github signup](https://github.com/user-attachments/assets/b994a539-7bd3-45a4-8fad-ddc967dbf12f)
![github username](https://github.com/user-attachments/assets/d47f235d-1b1d-47b8-bb40-4dd1b5daa292)


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

1. Open the GitHub repository you want to copy, click on the "Code" button, and copy the repository link.![cloning](https://github.com/user-attachments/assets/2cc9d54b-5ee3-46f0-83b0-ef14d0497427)

2. Create a folder on your computer where you want to clone the repository.
3. Open Git Bash and navigate to the folder you created using the command:

    ```bash
    cd <folder-directory>
    ```

4. Clone the repository by running:

    ```bash
    git clone <repository-link>
    ```

5. You have successfully cloned the repository!

---

### Step 4: Basic Git Commands
There are two ways to open a specific folder or repository:

cd <folder directory>

or right-click the folder on your computer, select "More options," and choose "Open Git Bash here" 
![open git bash](https://github.com/user-attachments/assets/544f594b-36fe-41c7-b199-0149549e8e82)

Here are some essential Git commands you'll use frequently:

| **Command**              | **Description**                                                             | **reference image**  |
|--------------------------|-----------------------------------------------------------------------------|-----------------------------|
| `git init`               | Initializes a new Git repository in the current directory.                  |![Screenshot 2025-01-11 133816](https://github.com/user-attachments/assets/28e1db67-fc12-4b64-97a4-64cb4d22e0bf)|
| `git status`             | Shows the status of your repository (e.g., changes, untracked files).       |![git status](https://github.com/user-attachments/assets/3ffca7c2-d566-49ff-ba58-e9c35b70ca24)|
| `git add <file>`         | Adds specific files to the staging area.                                    |![git add](https://github.com/user-attachments/assets/931ab7e0-d1a3-4ad3-9234-b140dcf2d338)|
| `git add .`              | Adds all changes in the directory to the staging area.                      |![git add2](https://github.com/user-attachments/assets/0e7e5771-c498-4372-842d-17d6c7df9fda)|
| `git commit -m "message"`| Saves changes to the repository with a descriptive message.                 |![git commit](https://github.com/user-attachments/assets/0a1e4735-0275-450d-8588-62d1aecae526)|
| `git log`                | Displays the commit history.                                                |![git log](https://github.com/user-attachments/assets/b94b0bde-8dab-412f-9841-bbbf8c6fe66c)|
| `git push`               | Pushes local changes to the remote repository.                              |![git push](https://github.com/user-attachments/assets/80df6330-6581-4b27-a4e7-9fba5102d325)|
| `git pull`               | Fetches and merges changes from the remote repository.                      |![git pull](https://github.com/user-attachments/assets/d5faa43b-01d7-40ee-a0ed-b0308843f144)
|

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
### Branching Workflow

At ChaiCode, we use a structured branching strategy to manage our projects effectively:

- **`main` branch**: The stable production branch.
- **`development` branch**: The integration branch for ongoing development.
- **Feature branches**: Separate branches for working on specific features or fixes. These branches are merged into `development` once complete.

#### Creating and Switching Branches

To create and switch to a new branch:

```bash
git branch feature/tea-menu
git checkout feature/tea-menu
```

Alternatively, use:

```bash
git checkout -b feature/tea-menu
```

#### Merging Branches

To merge a feature branch into `development`:

1. Switch to the `development` branch:

    ```bash
    git checkout development
    ```

2. Merge the feature branch:

    ```bash
    git merge feature/tea-menu
    ```

#### Resolving Conflicts

If there are merge conflicts:

1. Open the conflicting files and make the necessary edits.
2. Add the resolved files to the staging area:

    ```bash
    git add <file-name>
    ```

3. Commit the merge:

    ```bash
    git commit
    ```

---

### Creating a Pull Request (PR) on GitHub

A pull request (PR) is used to propose changes and collaborate on code reviews. Follow these steps to create a PR:

1. Push your branch to GitHub:

    ```bash
    git push origin <branch-name>
    ```
![creating new branch](https://github.com/user-attachments/assets/103f8fc5-a019-49de-9bae-dcf0e39f663d)
![git pull request 2](https://github.com/user-attachments/assets/1986bdca-0517-47b6-bb77-65def789a602)

![pull request](https://github.com/user-attachments/assets/379ca479-24bf-4fcf-873c-9c3f6e529a76)
4155-49e1-b941-094987b5ce73)


2. Go to the repository on GitHub and click on **Pull Requests**.
3. Click **New Pull Request**.
4. Select the base branch and compare branch.

#### Writing a PR Description

- Provide a clear and concise description of the changes.
- Include the purpose of the PR and any relevant context.
- Mention related issues or tasks using keywords like `Fixes #issue-number`.

#### Requesting Code Reviews

- Add reviewers who are familiar with the codebase or the changes.
- Highlight specific areas in the code that require attention.

*(Insert Screenshot Here)*

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
