# Standard Operating Procedure (SOP)  
**Installing Git on Windows System**  
**Date:** December 15, 2025  

---

### **Objective**  
To provide step-by-step instructions for installing Git on a Windows system, including configuration options for optimal use in development environments.  

---

### **Prerequisites**  
- Windows operating system (64-bit recommended)  
- Internet connection for download  
- Administrator privileges for installation  

---

### **Procedure**  

**Step 1: Download Git Installer**  
- Navigate to the official Git website: [https://git-scm.com/](https://git-scm.com/)  
- Click the **Windows download link** (latest version, e.g., Git 2.52.0 x64).  
- Save the installer (`Git-2.52.0-64-bit.exe`) to your computer.  

   ![git download](./images/image1.png)

---

**Step 2: Launch the Installer**  
- Locate the downloaded installer and double-click to run it.  
- If prompted by **User Account Control**, click **Yes** to allow changes.  

---

**Step 3: License Agreement**  
- Read the GNU General Public License.  
- Click **Next** to proceed.  

---

**Step 4: Select Destination Location**  

The **default** destination location for installing Git is set to the `C:\Program Files\Git` directory, which is the standard and recommended program installation path on Windows systems. You can click **Browse** to choose a different
- Accept the default installation folder:  
   ```
   C:\Program Files\Git
   ```  
- Click **Next**.  

   ![program location](./images/image2.png)


---

**Step 5: Select Components**  
- Choose the components to install (**recommended** selections by **default**):
  - [ ] Additional icons (optional)    
  - [x] **Windows Explorer integration**  
  - [x] **Git LFS (Large File Support)**  
  - [x] **Associate .git* configuration files with default text editor**  
  - [x] **Associate .sh files with Bash**  
  - [ ] Check daily for updates (optional)  
  - [ ] Add a Git Bash Profile to Windows Terminal  
  - [x] **Scalar** (for large-scale repositories)  

- Click **Next**.  

   ![program location](./images/image3.png)

---

**Step 6: Start Menu Folder**  
- Accept the default Start Menu folder or choose **Don’t create a Start Menu folder**.
- I choose to default which create a start menu folder for git.  
- Click **Next**.  

   ![program location](./images/image4.png)

---

**Step 7: Choose Default Editor**

The recommended setting is to select "Visual Studio Code" as the default editor for Git, which will be used for writing commit messages and other tasks. 

if you want you can choose different option for this from the dropdwon menu.

- Select **Use Visual Studio Code as Git’s default editor** (recommended).  
- Click **Next**.  
   
   ![program location](./images/image5.png)

---

**Step 8: Adjust Initial Branch Name**  

Select **Override the default branch name**, enter **main**, and click Next. This aligns with the modern standard, moving away from the old default of **master**.

- Select **Override the default branch name for new repositories**.  
- Enter **`main`** as the default branch name (recommended).  
- Click **Next**.  

   ![program location](./images/image6.png)

---

**Step 9: Adjust PATH Environment**

Select the option **Git from the command line and also from 3rd-party software**(Recommended) and click Next. This adds Git to your **system PATH**, allowing you to use it from any command prompt, terminal, or external application.

- Select:  
  - [x] **Git from the command line and also from 3rd-party software**  
  
- Click **Next**.  
   
   ![program location](./images/image7.png)

---

**Step 10: Choose SSH Executable**  

Select the default **"Use bundled OpenSSH"** and click Next. This uses the SSH client included with Git for **secure** connections with the **github** repository.

- Select **Use bundled OpenSSH** (default).  
- Click **Next**.

   ![program location](./images/image8.png)

---

**Step 11: Choose HTTPS Transport Backend**

Select the default **"Use the OpenSSL library"** and click Next. This handles **HTTPS** connections for **secure** repository access.

- Select:  
  - [x] **Use the OpenSSL library** (default).  

- Click **Next**.  

   ![program location](./images/image9.png)

---

**Step 12: Configure Line Ending Conversions**

Select **"Checkout Windows-style, commit Unix-style line endings"** and click Next. This ensures **compatibility** when working across **Windows** and **Unix systems** (like Linux/macOS).

- Select:  
  - [x] **Checkout Windows-style, commit Unix-style line endings** (recommended for cross-platform work).  

- Click **Next**.  

   ![program location](./images/image10.png)

---

**Step 13: Choose Terminal Emulator**

Select **"Use MinTTY"** and click Next. This provides a better terminal to use **git CLI** experience with resizing and improved font rendering.

- Select:  
  - [x] **Use MinTTY** (recommended for better terminal experience).  

- Click **Next**.  

   ![program location](./images/image11.png)

---

**Step 14: Configure `git pull` Behavior**  

Select the default option **"Fast-forward or merge"** and click Next.
This setting controls how git **pull** brings in **updates** from your **team**. Here’s what it does in simple terms:

1. If your branch is **behind**: It simply updates your work with the **latest** changes, like **fast-forwarding a video**.

2. If both you and your team have made **commits**: It safely combines both sets of changes and creates a **“merge commit”** that clearly shows where the **histories** came together.

This is the standard and safe way to keep your project in **sync**.

- Select:  
  - [x] **Fast-forward or merge** (default and recommended).  

- Click **Next**.  

   ![program location](./images/image12.png)

---

**Step 15: Choose Credential Helper**  

Select **"Git Credential Manager"** and click Next. This securely stores your **login credentials** for **Git** hosting services like GitHub.

- Select Git credential manager (recommended for secure credential storage):  
  - [x] **Git Credential Manager**

- Click **Next**.  

   ![program location](./images/image13.png)

---

**Step 16: Configure Extra Options**  
- Enable:  
  - [x] **Enable file system caching** (performance boost)  
  - [ ] **Enable symbolic links** (if supported by your system)  

- Click **Next**.
- 
   ![program location](./images/image14.png)

---

**Step 17: Begin Installation**  
1. Review settings.  
2. Click **Install**.  
3. Wait for installation to complete (progress bar will show).  

   ![program location](./images/image15.png)

---

**Step 18: Finish Installation**  
- Once installation is complete, check **Launch Git Bash** if desired.  
- Click **Finish**.  

---

### **Verification**  
1. Open **Command Prompt** or **Git Bash**.  
2. Run the following command to verify installation:  
   ```bash
   git --version
   ```  
3. Expected output:  
   ```
   git version 2.52.0
   ```  

---

### **Post-Installation Configuration**  
- Set your Git username and email (required for commits):
    
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```  

---

### **Troubleshooting**  
- If `git` is not recognized in Command Prompt, restart your terminal or system.  
- Ensure the **Git installation directory** is added to the system PATH (Step 9).  
  

---

### **References**  
- Official Git Documentation: [https://git-scm.com/doc](https://git-scm.com/doc)  
- Git for Windows Releases: [https://gitforwindows.org/](https://gitforwindows.org/)  

---

**End of SOP**