# EP-002 - Linux Navigation

**Series:** From Beginner to SOC Analyst

**Phase:** Linux Fundamentals

**Episode:** 002

**Topic:** Linux Navigation

**Status:** ✅ Completed

---

# 🎮 Mission

## CASE #002 - The Missing Evidence

A security alert reports multiple failed SSH login attempts.

Your senior analyst tells you that the evidence is stored inside:

```text
/var/log/auth.log
```

Your task is to reach that location using only terminal commands.

No mouse.

No graphical interface.

---

# 🎯 Objective

Learn how to navigate the Linux file system using the terminal.

---

# 🧠 Key Concepts Learned

- Current Working Directory
- Change Directory (`cd`)
- Root Directory (`/`)
- Home Directory (`~`)
- Current Directory (`.`)
- Parent Directory (`..`)
- Absolute Path
- Relative Path

---

# 💻 Commands Learned

- pwd
- ls
- ls -l
- cd
- cd ..
- cd ~
- cd /

> Detailed explanations are available in `Linux/linux_commands.md`.

---

# 🧪 Practical Lab

```bash
pwd

cd Documents

pwd

cd ..

pwd

cd /

pwd

cd ~

pwd

cd /var/log

pwd
```

---

# 📸 Screenshot Checklist

- Terminal showing `/var/log`
- Terminal showing `cd ~`
- Optional screen recording of the navigation commands

---

# 🛡️ SOC Perspective

Linux servers are often managed without a graphical interface.

Security analysts need to navigate quickly between log files, user directories, and configuration files during investigations.

Navigation is one of the first practical Linux skills used in a SOC environment.

---

# ⭐ Interview Questions

1. What does `cd` do?
2. What is an absolute path?
3. What is a relative path?
4. What does `~` represent?
5. What does `..` represent?
6. What is the root directory?

---

# 🧠 Things Recruiters Expect You to Remember

- `cd` changes directories.
- `pwd` shows your current location.
- `/` is the root directory.
- `~` is your home directory.
- `..` moves to the parent directory.
- Absolute paths begin with `/`.
- Relative paths begin from your current location.

---

Mission Complete ✅