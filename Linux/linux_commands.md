# Linux Commands

> A practical command reference for my cybersecurity journey.
>
> **Series:** From Beginner to SOC Analyst

---

# CMD-001 | pwd (Print Working Directory)

📌 Purpose

Shows the current directory you're working in.

🧾 Syntax

```bash
pwd
```

💡 Example

```bash
pwd
```

Output

```text
/home/arhaan
```

🛡️ SOC Use

Always verify your location before viewing, modifying, or collecting evidence.

⭐ Interview

Used to display the current working directory.

---

# CMD-002 | ls (List)

📌 Purpose

Lists files and directories.

🧾 Syntax

```bash
ls
```

💡 Common Usage

```bash
ls
ls Downloads
ls Desktop
```

🛡️ SOC Use

Used to discover files and folders during investigations.

⭐ Interview

`ls` shows names only.

---

# CMD-003 | ls -l (Long Listing)

📌 Purpose

Shows detailed information about files and directories.

🧾 Syntax

```bash
ls -l
```

💡 Displays

- Permissions
- Owner
- Group
- Size
- Date
- Filename

🛡️ SOC Use

Useful when checking file permissions or ownership.

⭐ Interview

Know what each column represents.

---

# CMD-004 | cd (Change Directory)

📌 Purpose

Move to another directory.

🧾 Syntax

```bash
cd <directory>
```

💡 Common Usage

```bash
cd Documents
cd Downloads
cd /var/log
```

🛡️ SOC Use

Navigate to logs, configuration files, and evidence locations.

⭐ Interview

Know the difference between absolute and relative paths.

---

# CMD-005 | cd ..

📌 Purpose

Move to the parent directory.

🧾 Syntax

```bash
cd ..
```

💡 Example

```bash
cd ..
```

🛡️ SOC Use

Quickly move up one directory while investigating.

⭐ Interview

`..` always means the parent directory.

---

# CMD-006 | cd ~

📌 Purpose

Return to the home directory.

🧾 Syntax

```bash
cd ~
```

🛡️ SOC Use

Quickly return to your user workspace.

⭐ Interview

`~` represents the current user's home directory.

---

# CMD-007 | cd /

📌 Purpose

Move to the root directory.

🧾 Syntax

```bash
cd /
```

🛡️ SOC Use

Start navigating from the top of the Linux file system.

⭐ Interview

`/` is the root directory, not the home directory.