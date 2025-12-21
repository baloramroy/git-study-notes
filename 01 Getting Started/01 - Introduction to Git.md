
# Introduction to Git

## Git

**What is Git?**

**Git** is a **Distributed Version Control System (DVCS)** used to **track changes in source code**, manage **multiple versions of files**, and enable **collaboration among developers or engineers**.

In simple terms:

* Git keeps a **complete history** of your project
* It allows you to **go back to any previous version**
* Multiple people can work on the **same project simultaneously**
* Changes can be **reviewed, compared, and merged safely**

>**Note:** Git was created by **Linus Torvalds** in **2005** to manage the Linux kernel source code efficiently.

## Why Git is important

* Prevents **accidental data loss**
* Makes **team collaboration easier**
* Helps in **auditing changes** (who changed what and when)
* Essential for **modern DevOps, Cloud, and CI/CD workflows**

As we came to know about **git** we also came to know another terms call **Version Control System**. Now the question arise what is version control system?

---

## Version Control System (VCS)?

**What is Version Control System?**

A **Version Control System** is a tool that:

* Tracks **changes to files over time**
* Maintains **multiple versions** of the same file
* Allows restoring files to a **previous state**
* Supports **collaboration** without overwriting others’ work

Without a VCS, managing code changes manually becomes **error-prone and unscalable**.

---

## Categories of Version Control Systems

Version Control Systems are mainly divided into **three categories**:

### 1. Local Version Control System

**Concept:**

A **Local Version Control** System is a **self-contained** version management tool that tracks **file revisions** exclusively on an **individual user's machine**.

* It maintains a **private database** of file **snapshots, changes, and history** without any networking
* No collaboration support

**How it works:**

* Changes are saved as copies or patches
* History is maintained only on that local system

**Example tools:**

* RCS (Revision Control System)

**Limitations:**

* No team collaboration
* High risk of data loss
* Not suitable for modern development

---

### 2. Centralized Version Control System (CVCS)

**Concept:**

In a **Centralized** version control system, all team members connect to a **central server** to get the latest copy of the code and to share their changes with others.
The **central repository** stores the complete project history, and users must communicate with this server to commit or update code.

**How it works:**

* One main repository on the central server
* Clients depend on the central server

**Example tools:**

* SVN (Subversion)
* CVS
* Perforce

**Advantages:**

* Simple to understand
* Centralized access control

**Limitations:**

* Single point of failure
* Requires network connectivity
* Slower for large teams

---

### 3. Distributed Version Control System (DVCS)

**Concept:**

In a **Distributed** version control system, each team member has a **full copy of the code and the entire repository** on their local machine.
Even if the central server goes offline, users can **continue working independently** and synchronize their changes later.

**How it works:**

* Each developer clones the full repository
* Work can be done even network goes **offline**
* Changes are synchronized when needed

**Example tools:**

* Git
* Mercurial

**Advantages:**
* No single point of failure
* High performance
* Offline work supported
* Strong collaboration and branching
* Very reliable and scalable

**Git belongs to this category.**

---

## Why Git is Preferred Today

* Industry standard for version control
* Used by platforms like **GitHub, GitLab, Bitbucket**
* Strong branching and merging capabilities
* Perfect fit for **DevOps and automation pipelines**

---



