# Standard Operating Procedure (SOP)  
**Installing Git on Linux System**  
**Date:** December 18, 2025  

---

### **Objective**  
To provide step-by-step instructions for installing **Git** on a Linux system using linux package manager.

---

### **Prerequisites**  
- **Linux** operating system  
- Internet connection for download  
- **Administrator** privileges for installation (root or sudo)

---

## Install Git Using Package Manager (Recommended)

### Install Git on RHEL / CentOS / Rocky / AlmaLinux

Step 1: Update system repositories
```bash
sudo dnf update -y
```
Step 2: Install Git
```bash
sudo dnf install git -y
```
Step 3: Verify installation
```bash
git --version
```

**Example output:** `git version 2.43.0`


### Install Git on Ubuntu / Debian

Step 1: Update package index
```bash
sudo apt update
```

Step 2: Install Git
```bash
sudo apt install git -y
```

Step 3: Verify installation
```bash
git --version
```