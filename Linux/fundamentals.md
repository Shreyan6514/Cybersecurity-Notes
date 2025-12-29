---

# ⚙️ Linux Fundamentals

Linux is a powerful open-source operating system used in servers, desktops, and embedded systems.

## 🔑 Key Concepts
- **Distributions:** Ubuntu, Debian, CentOS, Fedora
- **Shell:** Command-line interface (bash, zsh)
- **Filesystem:** /home, /etc, /var, /usr
- **Permissions:** `rwx` for files and directories
- **Users & Groups:** `adduser`, `usermod`, `groups`

---
## 📄 Basic Commands
```bash

echo     # Output any text that we provide
whoami   # Find out what user we're currently logged in as

ls           # List files
cd           # Change directory
cat          # Concatenate
pwd          # Print working directory
mkdir        # Make directory
rm           # Remove file or directory
chmod        # Change permissions

---

## 🔍 Searching Files & Text in Linux

Linux provides powerful command-line tools to search files and text inside files.

---

### 🗂 Searching for Files — `find`

`find` searches files by name, type, size, or path.

Find a file by name:

```bash
find / -name file.txt
```

Search in current directory:

```bash
find . -name notes.txt
```

Find all `.log` files:

```bash
find /var/log -name "*.log"
```

Find directories only:

```bash
find . -type d
```

Find files larger than 10MB:

```bash
find . -size +10M
```

---

### 🧾 Searching Inside Files — `grep`

`grep` searches for matching text patterns.

Find text inside a file:

```bash
grep "error" logfile.txt
```

Search recursively in folder:

```bash
grep -r "admin" .
```

Show line numbers:

```bash
grep -n "password" config.txt
```

Case-insensitive search:

```bash
grep -i "user" users.txt
```

Use regex search:

```bash
grep -E "[0-9]{3}-[0-9]{2}-[0-9]{4}" file.txt
```

---

## 🔗 Pipes (`|`) — Combining Commands

A pipe sends the **output of one command → into another command**.

Example:

```bash
ls -l | grep ".txt"
```

Meaning:

- `ls -l` lists files
- `grep ".txt"` filters only `.txt` files

View running processes containing “ssh”:

```bash
ps aux | grep ssh
```

Count lines in output:

```bash
cat file.txt | wc -l
```

Pipes are heavily used in:

- security tools
- log analysis
- scripting

---

## 📤 Input & Output Redirection

Redirect output to a file.

Overwrite file:

```bash
echo "hello" > file.txt
```

Append to file:

```bash
echo "new line" >> file.txt
```

Redirect input to program:

```bash
cat < file.txt
```

Save command output to file:

```bash
ls -l > files.txt
```

Send both stdout + stderr:

```bash
command > output.txt 2>&1
```

Useful in security logs & debugging.

---

## ⭐ Wildcards (Globbing)

Wildcards match multiple files.

| Symbol | Meaning |
|------|--------|
| `*` | any characters |
| `?` | single character |
| `[]` | character ranges |

Examples:

All `.txt` files:

```bash
ls *.txt
```

Files starting with `log`:

```bash
ls log*
```

Files with one-letter prefix:

```bash
ls ?.txt
```

Range match:

```bash
ls file[1-5].txt
```

---

## 🧮 Logical & Symbolic Operators

### ✔ Logical operators

AND:

```bash
command1 && command2
```

Second runs only if first succeeds.

OR:

```bash
command1 || command2
```

Second runs only if first fails.

Run commands sequentially:

```bash
command1 ; command2
```

---

### 🔗 Symbolic Links

Create symlink:

```bash
ln -s original.txt link.txt
```

View what a link points to:

```bash
ls -l
```

Symbolic links are like **shortcuts / pointers**.

---

📌 *This section extends Linux fundamentals with command-line search, operators, and shell productivity tools.*
