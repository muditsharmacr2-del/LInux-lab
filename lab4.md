# 🧪 Linux Lab – File Ownership & Permissions  

This lab walks you through creating users, groups, and managing file ownership using **`chown`** and related commands in Linux.  

---

## 🔖 Badges  
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)  
![Bash](https://img.shields.io/badge/Bash-121011?style=for-the-badge&logo=gnu-bash&logoColor=white)  
![Shell Scripting](https://img.shields.io/badge/Shell_Scripting-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)  

---

## 📌 Steps

### 1️⃣ Create a New User  
```bash
sudo useradd -m newuser


* `-m` → Creates a home directory at `/home/newuser`.

---

### 2️⃣ Create a New Group

```bash
sudo groupadd newgroup
```

---

### 3️⃣ Add User to Group

```bash
sudo usermod -aG newgroup newuser
```

* `-aG` → Appends the user to the group without removing existing ones.

---

### 4️⃣ Create a File (as current user)

```bash
touch testfile.txt
```

🔍 Check ownership:

```bash
ls -l testfile.txt
```

Example output:

```
-rw-r--r-- 1 ubuntu ubuntu 0 Aug 19 14:02 testfile.txt
```

---

### 5️⃣ Assign Ownership to `newuser:newgroup`

```bash
sudo chown newuser:newgroup testfile.txt
```

---

### 6️⃣ Verify Ownership

```bash
ls -l testfile.txt
```

Expected output:

```
-rw-r--r-- 1 newuser newgroup 0 Aug 19 14:02 testfile.txt
```

---

## 📸 Screenshot Example

![Ownership verification](s5.png)

---

## ✅ Key Takeaways

* **`useradd -m`** → Creates a new user with a home directory.
* **`groupadd`** → Creates a new group.
* **`usermod -aG`** → Adds user to group without affecting existing memberships.
* **`chown user:group file`** → Changes file ownership.
* **`ls -l`** → Verifies permissions & ownership.

---
---