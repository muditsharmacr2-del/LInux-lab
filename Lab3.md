

```markdown
```

██╗     ██╗███╗   ██╗██╗   ██╗██╗  ██╗     ██████╗ ███╗   ███╗
██║     ██║████╗  ██║██║   ██║██║ ██╔╝    ██╔═══██╗████╗ ████║
██║     ██║██╔██╗ ██║██║   ██║█████╔╝     ██║   ██║██╔████╔██║
██║     ██║██║╚██╗██║██║   ██║██╔═██╗     ██║   ██║██║╚██╔╝██║
███████╗██║██║ ╚████║╚██████╔╝██║  ██╗    ╚██████╔╝██║ ╚═╝ ██║
╚══════╝╚═╝╚═╝  ╚═══╝ ╚═════╝ ╚═╝  ╚═╝     ╚═════╝ ╚═╝     ╚═╝

````
# 🌟 Basic Linux Commands — A Visual & Practical Guide  

> **By:** Mudit Kumar Sharma  
> **OS:** Ubuntu  
> **Difficulty:** 🟢 Beginner  

Learning Linux is easier when you see **real outputs** and try them yourself.  
This guide covers **essential Linux commands** with **colored terminal examples** and **real screenshots** for clarity.

---

## 📍 1. `pwd` — Print Working Directory  

The `pwd` command displays your **current location** in the filesystem.

```bash
mudit@mudit-Inspiron-3505:~$ pwd
/home/mudit
````

💡 **Tip:** Always check your working directory before creating, deleting, or moving files.

🖼 **Screenshot:**
![pwd command output](./images/s1.png)

---

## 📂 2. `ls` — List Files & Directories

The `ls` command shows **files and folders** in your current directory.

```bash
mudit@mudit-Inspiron-3505:~$ ls
'C codes'   Desktop   LAB     Music      pROJECTS2  temp  
C_Lab       Documents Linux   Pictures   Public     Templates  
data1.txt   Downloads LINUX   Projects   snap       Videos
```

💡 **Tip:**

* **Blue** → Directories
* **Green** → Executable files
* **White** → Regular files
  *(Colors depend on your terminal theme.)*

🖼 **Screenshot:**
![ls command output](./images/s2.png)

---

### 🎯 2.1 Using Flags with `ls`

| Flag  | Description                                    |
| ----- | ---------------------------------------------- |
| `-l`  | Detailed view (permissions, owner, size, date) |
| `-a`  | Show hidden files (start with `.`)             |
| `-la` | Combine both views                             |

```bash
mudit@mudit-Inspiron-3505:~$ ls -la
total 132
drwxr-x--- 22 mudit mudit 4096 Aug 15 15:01 .
drwxr-xr-x  3 root  root  4096 Aug 10 00:22 ..
-rw-------  1 mudit mudit 6423 Aug 15 15:03 .bash_history
-rw-r--r--  1 mudit mudit  220 Mar  5 08:05 .bash_logout
-rw-r--r--  1 mudit mudit 3771 Mar  5 08:05 .bashrc
...
```

🖼 **Screenshot:**
![ls -la command output](./images/s3.png)

---

## 🧠 Quick Recap

| Command  | Purpose                      | Common Flags      |
| -------- | ---------------------------- | ----------------- |
| `pwd`    | Shows current directory      | *(none)*          |
| `ls`     | Lists files & directories    | `-l`, `-a`, `-la` |
| `ls -la` | Lists all files with details | *(most used)*     |

---

✨ **Pro Tip:** Chain commands for efficiency:

```bash
pwd && ls -la
```

This prints your **current path** and **detailed directory contents** in one go.

💻 **Challenge:** Try `ls -la` in `/etc` or `/var/log` to explore system configuration and log files.

---

```

---


