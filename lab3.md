Perfect 🙌 I see your **Lab-3 Part2.md** is a collection of Linux commands (sudo, user management, permissions, networking, package management, etc.). Right now, it looks like plain notes.

Let’s make it **most attractive, engaging, and easy to understand** by:

* Adding **clear sections with emojis & headings**
* Using **callouts / tips** for important notes
* Keeping commands inside **well-formatted code blocks**
* Adding **tables & explanations** where needed

Here’s a **revamped version of your MD file** 👇

````markdown
# 🚀 Linux Intermediate & Advanced Commands Guide  

Welcome! This guide covers **essential Linux commands** for system administration, user management, networking, and more.  
It’s designed to be **clear, engaging, and beginner-friendly** 🎯  

---

## 🔑 1. Run Commands as Administrator (`sudo`)  

`sudo` = **SuperUser DO** → allows you to run commands with **root privileges**.  

```bash
sudo command
````

✅ Examples:

```bash
sudo apt update      # Run package update as admin  
sudo reboot          # Reboot system  
```

⚡ **Tip:** You’ll usually be prompted to enter your password.

---

## 👥 2. User Management

### ➕ Add a New User

```bash
sudo adduser newusername
```

### 🔑 Change User Password

```bash
sudo passwd newusername
```

### 📝 Modify User (Add to Group)

```bash
sudo usermod -aG groupname username
```

Example:

```bash
sudo usermod -aG sudo alice   # Give 'alice' sudo access  
```

### ❌ Delete a User

```bash
sudo deluser username
sudo deluser --remove-home username   # Remove user + home directory  
```

---

## 🔐 3. File Permissions & Ownership

### `chmod` → Change File Permissions

```bash
chmod [permissions] file
```

Examples:

```bash
chmod 755 script.sh   # Owner: read/write/execute; Others: read/execute  
chmod +x file.sh      # Add execute permission  
chmod -x file.sh      # Remove execute permission  
```

📊 **Permission Table:**

| Number | Permission Type        |
| ------ | ---------------------- |
| 7      | read + write + execute |
| 6      | read + write           |
| 5      | read + execute         |
| 4      | read only              |
| 0      | no permission          |

---

### `chown` → Change File Owner

```bash
sudo chown user:group file
```

Example:

```bash
sudo chown alice:alice myfile.txt
```

---

## 💽 4. Disk Usage & System Info

* **Disk Space Usage**

```bash
df -h
```

* **Folder Size**

```bash
du -sh folder_name
```

* **Live System Processes**

```bash
top   # Press 'q' to quit
```

💡 Use `htop` (better UI) → install with:

```bash
sudo apt install htop
```

---

## 🌐 5. Networking Commands

* **Ping a Website**

```bash
ping google.com
```

* **Check IP & Network Info**

```bash
ip a
ifconfig   # (may require sudo or installation)
```

* **Show Active Connections**

```bash
netstat -tuln
ss -tuln   # Faster alternative
```

---

## 📦 6. Package Management

### For **Ubuntu/Debian (APT)**

```bash
sudo apt update            # Refresh package list  
sudo apt upgrade           # Upgrade installed packages  
sudo apt install git       # Install a package  
sudo apt remove git        # Uninstall a package  
```

### For **macOS (Homebrew)**

```bash
brew install git
```

---

## ⚙️ 7. Process Management

* **Show Running Processes**

```bash
ps aux
```

* **Kill a Process**

```bash
kill <PID>
```

Example:

```bash
kill 12345
kill -9 12345   # Force kill  
```

---

## 🔌 8. Shutdown & Reboot

```bash
sudo shutdown now        # Immediate shutdown  
sudo shutdown -r now     # Immediate reboot  
```

---

✨ **Pro Tip:** Practice these commands on a safe test system or VM.
They are powerful and can change your system configuration 🔧

---

✅ Now your notes are **professional, structured, and beginner-friendly** 🎉

```

---

Do you want me to also **add some Ubuntu terminal screenshots** (like `ls`, `top`, `htop`) inside the markdown so it becomes **visual + explanatory** for your GitHub?
```
