Got it ✅ You want me to create a **good-looking, engaging, interesting Markdown (`.md`) file** for a **Shell Scripting tutorial**.
Here’s a professional and attractive one you can directly use in your GitHub repo:

---

````markdown
# 🐚 Shell Scripting Tutorial  

Welcome to the **Shell Scripting Tutorial** 🚀  
This guide will help you learn Linux shell commands and scripting in an **engaging and practical way**.  

---

## 📌 What is Shell Scripting?  
A **Shell Script** is simply a file with a series of commands written in the **Linux shell language** (like `bash`).  
It allows you to:  
- ✅ Automate repetitive tasks  
- ✅ Save time and effort  
- ✅ Create your own commands  

---

## ⚡ Basic Linux Commands  

| Command       | Description                        | Example Output |
|---------------|------------------------------------|----------------|
| `whoami`      | Shows current logged-in user       | `mudit` |
| `pwd`         | Prints current working directory   | `/home/mudit` |
| `ls`          | Lists files & directories          | `file1 file2 dir1` |
| `echo`        | Prints text/message                | `echo "Hello World"` → `Hello World` |

---

## 🛠️ Writing Your First Shell Script  

1. Create a new file:  
   ```bash
   nano hello.sh
````

2. Add this code:

   ```bash
   #!/bin/bash
   echo "Hello, World! 🚀"
   ```

3. Save and exit (`CTRL + O`, `CTRL + X`).

4. Give execute permission:

   ```bash
   chmod +x hello.sh
   ```

5. Run the script:

   ```bash
   ./hello.sh
   ```

✅ Output:

```
Hello, World! 🚀
```

---

## 🔑 File Permissions (Quick Guide)

| Number | Permission             | Symbol |
| ------ | ---------------------- | ------ |
| `7`    | Read + Write + Execute | `rwx`  |
| `6`    | Read + Write           | `rw-`  |
| `5`    | Read + Execute         | `r-x`  |
| `4`    | Read only              | `r--`  |
| `0`    | No permission          | `---`  |

👉 Example:

```bash
chmod 755 hello.sh
```

Means: Owner = `rwx`, Group = `r-x`, Others = `r-x`.

---

## 🔄 Example Script – Loop

```bash
#!/bin/bash
for i in 1 2 3 4 5
do
  echo "Iteration $i"
done
```

✅ Output:

```
Iteration 1
Iteration 2
Iteration 3
Iteration 4
Iteration 5
```

---

## 🎯 Next Steps

* Learn about **variables & conditions (`if-else`)**
* Practice **loops** (`for`, `while`, `until`)
* Explore **functions** in shell scripting

---

## 🌟 Pro Tip

Always start your script with:

```bash
#!/bin/bash
```

This is called a **shebang**, and it tells Linux to run the file using `bash`.

---

