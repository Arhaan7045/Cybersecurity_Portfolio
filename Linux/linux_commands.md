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

View large text files one screen at a time.

🧾 Example

```bash
less /var/log/syslog
```

🛡️ SOC Use

Safely examine large log files without dumping everything onto the terminal.

Press `q` to exit.

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

Display the end of a text file.

🧾 Example

```bash
tail -n 20 /var/log/syslog
```

🛡️ SOC Use

Quickly inspect recent entries in a log file.

---

# CMD-018 | grep

📌 Purpose

Search text for a specific pattern.

🧾 Example

```bash
grep "Failed" /var/log/auth.log
```

🛡️ SOC Use

Find specific events or keywords inside logs.

⭐ Interview

Very useful for filtering large amounts of log data.

# CMD-019 | chmod (Change Mode)

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

# CMD-020 | chown (Change Owner)

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

# CMD-021 | chgrp (Change Group)

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

# CMD-022 | whoami

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

# CMD-023 | id

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

# CMD-024 | groups

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

# CMD-025 | who

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

# CMD-026 | sudo

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

---

# CMD-027 | ps

📌 Purpose

Display currently running processes.

🧾 Syntax

```bash
ps
```

💡 Common Usage

```bash
ps
```

🛡️ SOC Use

Quickly inspect processes running in the current session.

⭐ Interview

Provides a snapshot of processes.

---

# CMD-028 | ps aux

📌 Purpose

Display detailed information about running processes.

🧾 Syntax

```bash
ps aux
```

💡 Important Columns

- USER
- PID
- %CPU
- %MEM
- STAT
- COMMAND

🛡️ SOC Use

Investigate processes, their owners, and resource usage.

⭐ Interview

Know what USER, PID, %CPU and COMMAND represent.

---

# CMD-029 | top

📌 Purpose

Display a continuously updating view of running processes and system resource usage.

🧾 Syntax

```bash
top
```

💡 Common Usage

```bash
top
```

Press:

```text
q
```

to exit.

🛡️ SOC Use

Monitor CPU and memory usage and identify processes consuming unusual resources.

⭐ Interview

`ps` is a snapshot; `top` is a live view.

---

# CMD-030 | kill

📌 Purpose

Send a signal to a process.

🧾 Syntax

```bash
kill <PID>
```

💡 Common Usage

```bash
kill 4210
```

🛡️ SOC Use

Terminate a process when appropriate during system administration or incident response.

⭐ Interview

The default signal is SIGTERM (15), which requests graceful termination.

---

# CMD-031 | killall

📌 Purpose

Send a signal to processes matching a name.

🧾 Syntax

```bash
killall <process_name>
```

💡 Example

```bash
killall firefox
```

🛡️ SOC Use

Can terminate multiple processes with the same name.

⚠️ Use carefully because multiple processes may be affected.

⭐ Interview

`kill` normally targets a PID; `killall` targets processes by name.

---

# CMD-032 | systemctl status

📌 Purpose

Check the current status of a system service.

🧾 Example

```bash
systemctl status ssh
```

🛡️ SOC Use

Investigate whether a service is running and inspect basic service information.

---

# CMD-033 | systemctl list-units

📌 Purpose

List currently loaded service units.

🧾 Example

```bash
systemctl list-units --type=service
```

🛡️ SOC Use

Review services currently managed by systemd.

---

# CMD-034 | systemctl start

📌 Purpose

Start a service immediately.

🧾 Example

```bash
sudo systemctl start ssh
```

---

# CMD-035 | systemctl stop

📌 Purpose

Stop a service immediately.

🧾 Example

```bash
sudo systemctl stop <service>
```

⚠️ Use carefully because stopping critical services can affect the system.

---

# CMD-036 | systemctl restart

📌 Purpose

Restart a service.

🧾 Example

```bash
sudo systemctl restart <service>
```

🛡️ SOC Use

Restart services after configuration changes when appropriate.

---

# CMD-037 | systemctl enable

📌 Purpose

Configure a service to start automatically during system boot.

🧾 Example

```bash
sudo systemctl enable ssh
```

---

# CMD-038 | systemctl disable

📌 Purpose

Prevent a service from automatically starting during system boot.

🧾 Example

```bash
sudo systemctl disable <service>
```

🛡️ SOC Use

Can be used when safely removing unwanted persistence or disabling unnecessary services.

---

# CMD-039 | journalctl

📌 Purpose

Read logs collected by the systemd journal.

🧾 Example

```bash
journalctl
```

🛡️ SOC Use

Review system events during investigations.

---

# CMD-040 | journalctl -n

📌 Purpose

Show the most recent journal entries.

🧾 Example

```bash
journalctl -n 20
```

🛡️ SOC Use

Quickly review recent system activity.

---

# CMD-041 | journalctl -b

📌 Purpose

Show journal entries from the current system boot.

🧾 Example

```bash
journalctl -b
```

🛡️ SOC Use

Investigate events that occurred since the system started.

---

# CMD-042 | journalctl -u

📌 Purpose

Show logs for a specific systemd service.

🧾 Example

```bash
journalctl -u ssh
```

🛡️ SOC Use

Investigate activity and errors related to a specific service.

---
