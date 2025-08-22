Here’s a polished and aesthetic **Markdown file** you can directly use in your GitHub repo. It’s engaging, well-structured, and styled for readability.

---

````markdown
# 🐚 Shell Tutorial – Mastering File Permissions with `chmod` and `chown`

Welcome to this tutorial!  
If you’ve ever wondered **"Why can’t I access or edit this file?"**, then this guide is for you.  
In Linux/Unix, **file permissions** control **who can read, write, or execute files**.  
We’ll explore `chmod` and `chown`—the essential commands to master file ownership and permissions.

---

## 📂 Understanding File Permissions

Each file or directory has **three types of permissions**:

| Permission | Symbol | Meaning |
|------------|--------|---------|
| Read       | `r`    | View file content / list directory |
| Write      | `w`    | Modify file / add or remove directory contents |
| Execute    | `x`    | Run the file (if it’s a script/program) / enter directory |

These permissions are assigned to **three categories of users**:

| User Type | Symbol | Who They Are |
|-----------|--------|--------------|
| Owner     | `u`    | The user who owns the file |
| Group     | `g`    | Users in the same group as the owner |
| Others    | `o`    | Everyone else |

---

## 🔎 Checking File Permissions

Use the `ls -l` command:

```bash
ls -l
````

Example output:

```
-rwxr--r--  1 mudit users  4096 Aug 21  file.sh
```

Breakdown:

* `-rwxr--r--` → File permissions
* `mudit` → File owner
* `users` → Group

So here:

* Owner can **read, write, execute**
* Group can **read**
* Others can **read**

---

## ⚡ `chmod` – Change File Permissions

The `chmod` command is used to **modify file permissions**.

### 1. Symbolic Mode

```bash
chmod u+x file.sh
```

✅ Adds **execute permission** for the owner.

```bash
chmod g-w file.txt
```

✅ Removes **write permission** for the group.

```bash
chmod o=r file.txt
```

✅ Sets **read-only** for others.

---

### 2. Numeric (Octal) Mode

Permissions are represented by numbers:

* `r = 4`, `w = 2`, `x = 1`

| Permission Set | Value |
| -------------- | ----- |
| `rwx`          | 7     |
| `rw-`          | 6     |
| `r-x`          | 5     |
| `r--`          | 4     |
| `---`          | 0     |

Example:

```bash
chmod 755 script.sh
```

* Owner → `7` (rwx)
* Group → `5` (r-x)
* Others → `5` (r-x)

---

## 👑 `chown` – Change File Ownership

The `chown` command is used to **change the owner or group** of a file.

### Change Owner

```bash
sudo chown mudit file.txt
```

✅ Makes `mudit` the owner of `file.txt`.

### Change Owner & Group

```bash
sudo chown mudit:devs project/
```

✅ Sets `mudit` as the owner and `devs` as the group for the `project/` directory.

---

## 🎯 Practical Examples

1. Make a script executable only by the owner:

```bash
chmod 700 secret.sh
```

2. Allow group collaboration on a directory:

```bash
chmod 770 project/
```

3. Transfer file ownership:

```bash
sudo chown newuser:newgroup report.docx
```

---

## 🧠 Quick Tips

* Use **symbolic mode** for small adjustments (`chmod u+x`).
* Use **numeric mode** for setting full permissions quickly (`chmod 644`).
* Always check with:

  ```bash
  ls -l
  ```
* Be cautious with `777` – it gives **everyone full access**. ⚠️

---

## 📌 Cheatsheet

| Task                    | Command                      |
| ----------------------- | ---------------------------- |
| Add execute for owner   | `chmod u+x file.sh`          |
| Remove write for group  | `chmod g-w file.txt`         |
| Give full access to all | `chmod 777 file`             |
| Change file owner       | `sudo chown user file`       |
| Change owner & group    | `sudo chown user:group file` |

---

## 🚀 Conclusion

By mastering `chmod` and `chown`, you gain **full control over file security and collaboration** in Linux.
Practice these commands regularly, and soon they’ll become second nature.

> 📝 Pro Tip: Always give the **minimum required permissions** for safety!

---

💡 *Happy Shell Scripting!* 🐧

```

-