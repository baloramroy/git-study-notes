
# Git Initial Configuration - After First Installation

## Git Configuration Levels

Git allows configuration at **three different levels**.
Understanding this prevents confusion later.

i. System Level

- Applies to **all users** on the computer
- Requires **administrator/root privileges**

ii. Global Level (Most Common)

- Applies to **all repositories of the current user**
- This is what we usually use for personal configuration

iii. Local Level

- Applies to **only the current repository**
- Overrides system and global settings


## Git Initial Configuration (Recommended)

### Linux / macOS Configuration

- Verify Git Installation

    ```bash
    git --version
    ```

    **Why:** Ensure Git is installed correctly.


- Configure Username (Global)

    ```bash
    git config --global user.name "Your Full Name"
    ```

    **Why:** Git records this name in every commit.


- Configure Email (Global)

    ```bash
    git config --global user.email "you@example.com"
    ```
    **Why:** Commit ownership and GitHub/GitLab mapping depend on this.


- Set Default Branch Name

    ```bash
    git config --global init.defaultBranch main
    ```
    **Why:** Modern Git standards use `main` instead of `master`.

- Set Default Editor
    
    ```bash
    git config --global core.editor nano
    ```
    **Why:** Git opens this editor for commit messages and rebases.

    **Note:** You can replace `nano` with `vim`.


- Enable Colored Output

    ```bash
    git config --global color.ui auto
    ```
    **Why:** Improves readability of status, diff, and logs.


- Line Ending Handling (Linux/macOS)

    ```bash
    git config --global core.autocrlf input
    ```
    **Why:** Prevents Windows line endings from breaking scripts.

- Configure Pull Strategy

    ```bash
    git config --global pull.rebase false
    ```
    **Why:** Prevents warnings and controls history behavior.

- Verify All Global Settings

    ```bash
    git config --global --list
    ```
---

### Windows Configuration

- Verify Git Installation

    ```bash
    git --version
    ```


- Configure Username

    ```bash
    git config --global user.name "Your Full Name"
    ```


- Configure Email

    ```bash
    git config --global user.email "you@example.com"
    ```

- Set Default Editor (Windows-Friendly)

    ```bash
    # If using Notepad:
    git config --global core.editor notepad

  # If using VS Code:
    git config --global core.editor "code --wait"
    ```

- Verify All Global Settings

    ```bash
    git config --global --list
    ```

**Note:** For windows, other configuration automatically get configured during the time of installation. 


---

## Minimal Required Configuration (All OS)

- If nothing else, **these two are mandatory**:

    ```bash
    git config --global user.name "Your Name"
    git config --global user.email "you@example.com"
    ```

---

## Optional but Useful Git Aliases

- Set aliases for daily use git command:

    ```bash
    git config --global alias.st status
    git config --global alias.co checkout
    git config --global alias.br branch
    git config --global alias.cm commit
    ```

    **Why:** Saves time for daily commands.

- Usage example:

    ```bash
    git st
    git cm -m "initial commit"
    ```

---

## Where Git Stores Configuration Files

| Level  | File Location    |
| ------ | ---------------- |
| System | `/etc/gitconfig` |
| Global | `~/.gitconfig`   |
| Local  | `.git/config`    |

---

