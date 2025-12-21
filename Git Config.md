## 1. Git Configuration Levels (Very Important to Understand)

Git allows configuration at **three different levels**.
Understanding this prevents confusion later.

### 1.1 System Level

• Applies to **all users** on the computer
• Requires **administrator/root privileges**

```bash
git config --system <key> <value>
```

Config file location:

```
/etc/gitconfig
```

Use case:
• Company-wide default settings
• Shared lab or server machines

---

### 1.2 Global Level (Most Common)

• Applies to **all repositories of the current user**
• This is what we usually use for personal configuration

```bash
git config --global <key> <value>
```

Config file location:

```
~/.gitconfig
```

Use case:
• Username
• Email
• Editor
• Aliases

---

### 1.3 Local Level

• Applies to **only the current repository**
• Overrides system and global settings

```bash
git config --local <key> <value>
```

Config file location:

```
<repo>/.git/config
```

Use case:
• Different email for work/project
• Special repo-specific behavior

---