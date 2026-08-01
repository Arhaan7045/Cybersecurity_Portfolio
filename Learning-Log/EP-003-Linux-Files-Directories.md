# EP-003 - Linux Files & Directory Operations

**Series:** From Beginner to SOC Analyst

**Phase:** Linux Fundamentals

**Episode:** 003

**Topic:** Linux Files & Directory Operations

**Status:** ✅ Completed

---

# 🎮 Mission

## CASE #003 - The Shadow File

Falcon Technologies detected suspicious file activity on a Linux server.

Before investigating the suspicious file, I learned how to safely create, copy, rename, move and remove files without touching production evidence.

---

# 🎯 Objective

Learn the most common Linux file and directory operations used by Linux administrators and SOC analysts.

---

# 🧠 Key Concepts Learned

- Creating directories
- Creating files
- Copying files
- Moving files
- Renaming files
- Deleting files
- Deleting empty directories

---

# 💻 Commands Learned

- mkdir
- touch
- cp
- mv
- rm
- rmdir

> Detailed command reference is available in `Linux/linux_commands.md`.

---

# 🧪 Practical Lab

Completed the following tasks:

- Created investigation folders
- Created suspicious files
- Copied evidence
- Renamed files
- Moved reports
- Deleted copied evidence
- Removed empty folders

---

# 🛡️ SOC Perspective

During an incident response, analysts rarely work on the original evidence.

Instead, they:

- Preserve the original file.
- Create a copy.
- Perform analysis on the copy.
- Keep investigation folders organized.

Good file management reduces mistakes and protects evidence.

---

# ⭐ Interview Questions

### 1. What is the difference between `mkdir` and `touch`?

### 2. What is the difference between `cp` and `mv`?

### 3. Why is `rm` considered dangerous?

### 4. What is the purpose of `rmdir`?

### 5. Why should analysts avoid modifying original evidence?

---

# 📸 Screenshots

- Investigation folders created
- Files created
- Files copied
- Files renamed
- Reports directory
- Successful mini mission

---

# 🧠 Things Recruiters Expect You To Remember

- `mkdir` creates directories.
- `touch` creates empty files.
- `cp` copies while preserving the original.
- `mv` moves or renames files.
- `rm` permanently deletes files.
- `rmdir` deletes only empty directories.
- Never analyze original evidence directly.

---

# Biggest Challenge

Remembering when to use `cp` versus `mv`.

---

# Biggest Takeaway

Good file management is essential during security investigations because preserving evidence is just as important as finding it.

---

# Next Episode

Viewing and Searching Files

Commands:

- cat
- less
- head
- tail
- grep

Mission:

Investigate a suspicious authentication log.