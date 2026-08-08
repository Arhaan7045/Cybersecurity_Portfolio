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

---

# CMD-008 | mkdir (Make Directory)

📌 Purpose

Create a new directory.

🧾 Syntax

```bash
mkdir <directory_name>
```

💡 Common Usage

```bash
mkdir Investigation
mkdir Reports
mkdir Evidence
```

🛡️ SOC Use

Create folders for evidence, reports and malware samples.

⭐ Interview

Creates directories only.

---

# CMD-009 | touch

📌 Purpose

Create an empty file.

🧾 Syntax

```bash
touch <file_name>
```

💡 Common Usage

```bash
touch report.txt
touch notes.txt
touch malware.sh
```

🛡️ SOC Use

Create reports, notes and test files.

⭐ Interview

Creates an empty file if it doesn't already exist.

---

# CMD-010 | cp (Copy)

📌 Purpose

Copy files or directories.

🧾 Syntax

```bash
cp <source> <destination>
```

💡 Common Usage

```bash
cp report.txt report_backup.txt
cp notes.txt Reports/
```

🛡️ SOC Use

Always copy evidence before analysis.

⭐ Interview

`cp` preserves the original.

---

# CMD-011 | mv (Move)

📌 Purpose

Move or rename files.

🧾 Syntax

```bash
mv <source> <destination>
```

💡 Common Usage

```bash
mv notes.txt analyst_notes.txt
mv analyst_notes.txt Reports/
```

🛡️ SOC Use

Rename suspicious files and organize investigation data.

⭐ Interview

Used for both moving and renaming.

---

# CMD-012 | rm (Remove)

📌 Purpose

Delete files.

🧾 Syntax

```bash
rm <file_name>
```

💡 Common Usage

```bash
rm notes.txt
rm report.txt
```

🛡️ SOC Use

Remove temporary files after confirming they are no longer needed.

⭐ Interview

Deletes permanently (no Recycle Bin).

---

# CMD-013 | rmdir (Remove Directory)

📌 Purpose

Delete an empty directory.

🧾 Syntax

```bash
rmdir <directory_name>
```

💡 Common Usage

```bash
rmdir EmptyFolder
```

🛡️ SOC Use

Clean up empty investigation folders.

⭐ Interview

Works only on empty directories.

---

# CMD-014 | cat

📌 Purpose

Display the contents of a file.

🧾 Syntax

```bash
cat <file>
```

💡 Common Usage

```bash
cat auth.log
cat notes.txt
```

🛡️ SOC Use

Quickly read configuration files and logs.

⭐ Interview

Displays the entire file at once.

---

# CMD-015 | less

📌 Purpose

View large files page by page.

🧾 Syntax

```bash
less <file>
```

💡 Common Usage

```bash
less auth.log
```

🛡️ SOC Use

Read large log files efficiently.

⭐ Interview

Press `q` to quit.

---

# CMD-016 | head

📌 Purpose

Display the first lines of a file.

🧾 Syntax

```bash
head <file>
head -n <file>
```

💡 Common Usage

```bash
head auth.log
head -3 auth.log
```

🛡️ SOC Use

Quickly inspect the beginning of logs.

⭐ Interview

Shows the first 10 lines by default.

---

# CMD-017 | tail

📌 Purpose

Display the last lines of a file.

🧾 Syntax

```bash
tail <file>
tail -n <file>
```

💡 Common Usage

```bash
tail auth.log
tail -2 auth.log
```

🛡️ SOC Use

Check the latest log entries during incident response.

⭐ Interview

Shows the last 10 lines by default.

---

# CMD-018 | grep

📌 Purpose

Search for text matching a pattern inside a file.

🧾 Syntax

```bash
grep <pattern> <file>
```

💡 Common Usage

```bash
grep Failed auth.log
grep Accepted auth.log
grep admin auth.log
```

🛡️ SOC Use

Search logs for failed logins, IP addresses, usernames, or error messages.

⭐ Interview

One of the most important Linux commands for SOC analysts.

---

# CMD-019 | ls -l (Deep Dive)

📌 Purpose

Display detailed information about files, including permissions, owner, group, size, and last modified date.

🧾 Syntax

```bash
ls -l
```

💡 Common Usage

```bash
ls -l
ls -l Documents
ls -l /var/log
```

🛡️ SOC Use

Check file permissions, ownership, and identify files that may be overly permissive or suspicious.

⭐ Interview

Be able to explain each part of a permission string such as:

```text
-rw-r--r--
```

---

# CMD-020 | chmod (Change Mode)

📌 Purpose

Change file or directory permissions.

🧾 Syntax

```bash
chmod <permissions> <file>
```

💡 Common Usage

```bash
chmod 755 backup.sh
chmod 644 report.txt
chmod +x script.sh
chmod u+x script.sh
chmod g-w script.sh
chmod o-x script.sh
```

🛡️ SOC Use

Secure files by applying the principle of least privilege and preventing unauthorized modification or execution.

⭐ Interview

Know the difference between numeric (755) and symbolic (u+x) permissions.

---

# CMD-021 | chown (Change Owner)

📌 Purpose

Change the owner of a file or directory.

🧾 Syntax

```bash
sudo chown <owner> <file>
```

💡 Common Usage

```bash
sudo chown root backup.sh
```

🛡️ SOC Use

Transfer ownership of sensitive files to the correct user.

⭐ Interview

Changes the file owner.

---

# CMD-022 | chgrp (Change Group)

📌 Purpose

Change the group ownership of a file or directory.

🧾 Syntax

```bash
sudo chgrp <group> <file>
```

💡 Common Usage

```bash
sudo chgrp developers backup.sh
```

🛡️ SOC Use

Grant access to the appropriate team without changing the file owner.

⭐ Interview

Changes only the group ownership.

---

# CMD-023 | whoami

📌 Purpose

Display the current logged-in username.

🧾 Syntax

```bash
whoami
```

🛡️ SOC Use

Verify which account is currently being used before performing administrative actions.

⭐ Interview

Shows only the username.

---

# CMD-024 | id

📌 Purpose

Display user ID (UID), group ID (GID), and group memberships.

🧾 Syntax

```bash
id
```

🛡️ SOC Use

Verify user identity and privileges during investigations.

⭐ Interview

Provides more information than `whoami`.

---

# CMD-025 | groups

📌 Purpose

Display all groups the current user belongs to.

🧾 Syntax

```bash
groups
```

🛡️ SOC Use

Check group memberships when troubleshooting permission issues.

⭐ Interview

Useful for understanding access rights.

---

# CMD-026 | who

📌 Purpose

Display users currently logged into the system.

🧾 Syntax

```bash
who
```

🛡️ SOC Use

Identify active user sessions during investigations.

⭐ Interview

May show no output on a personal desktop session, depending on how you're logged in.

---

# CMD-027 | sudo

📌 Purpose

Run a command with administrative (root) privileges.

🧾 Syntax

```bash
sudo <command>
```

💡 Common Usage

```bash
sudo apt update
sudo apt upgrade
sudo ls /root
```

🛡️ SOC Use

Perform administrative tasks while following the principle of least privilege.

⭐ Interview

Temporarily elevates privileges for a single command.