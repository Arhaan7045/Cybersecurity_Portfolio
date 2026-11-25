# Linux Commands

A practical reference for Linux commands covered in the cybersecurity learning episodes.

---

# CMD-001 | pwd

**Purpose**

Display the current working directory.

**Syntax**
```bash
pwd
```

**SOC Use**

Verify the current location before viewing, modifying or collecting files.

---

# CMD-002 | ls

**Purpose**

List files and directories.

**Syntax**
```bash
ls
```

**SOC Use**

Discover files and directories during system inspection.

---

# CMD-003 | ls -l

**Purpose**

Display detailed file and directory information, including permissions, owner, group, size and modification time.

**Syntax**
```bash
ls -l
```

**SOC Use**

Inspect permissions and ownership during file-access investigations.

---

# CMD-004 | cd

**Purpose**

Change the current directory.

**Syntax**
```bash
cd <directory>
```

**SOC Use**

Navigate to log locations, configuration directories and evidence folders.

---

# CMD-005 | cd ..

**Purpose**

Move to the parent directory.

**Syntax**
```bash
cd ..
```

**SOC Use**

Move between directory levels while navigating an investigation workspace.

---

# CMD-006 | cd ~

**Purpose**

Move to the current user's home directory.

**Syntax**
```bash
cd ~
```

**SOC Use**

Return to the analyst's home workspace.

---

# CMD-007 | cd /

**Purpose**

Move to the filesystem root directory.

**Syntax**
```bash
cd /
```

**SOC Use**

Begin navigation from the top level of the Linux filesystem.

---

# CMD-008 | mkdir

**Purpose**

Create a directory.

**Syntax**
```bash
mkdir <directory_name>
```

**SOC Use**

Create organised folders for reports, evidence and investigation files.

---

# CMD-009 | touch

**Purpose**

Create an empty file or update its timestamps if it already exists.

**Syntax**
```bash
touch <file_name>
```

**SOC Use**

Create notes or placeholder files for an investigation.

---

# CMD-010 | cp

**Purpose**

Copy files or directories.

**Syntax**
```bash
cp <source> <destination>
```

**SOC Use**

Preserve an original file by making a working copy before analysis.

---

# CMD-011 | mv

**Purpose**

Move or rename files and directories.

**Syntax**
```bash
mv <source> <destination>
```

**SOC Use**

Organise investigation files and rename working copies.

---

# CMD-012 | rm

**Purpose**

Remove files.

**Syntax**
```bash
rm <file_name>
```

**SOC Use**

Remove files only after confirming they are no longer required; deletion can affect evidence.

---

# CMD-013 | rmdir

**Purpose**

Remove an empty directory.

**Syntax**
```bash
rmdir <directory_name>
```

**SOC Use**

Remove empty temporary investigation directories.

---

# CMD-014 | cat

**Purpose**

Display the contents of a file.

**Syntax**
```bash
cat <file>
```

**SOC Use**

Quickly read short configuration files and log files.

---

# CMD-015 | less

**Purpose**

View a text file interactively one screen at a time.

**Syntax**
```bash
less <file>
```

**SOC Use**

Examine large logs without printing the entire file at once. Press q to exit.

---

# CMD-016 | head

**Purpose**

Display the first lines of a file.

**Syntax**
```bash
head <file>
head -n 3 <file>
```

**SOC Use**

Inspect the beginning of a log or text file.

---

# CMD-017 | tail

**Purpose**

Display the last lines of a file.

**Syntax**
```bash
tail <file>
tail -n 20 <file>
```

**SOC Use**

Inspect recent log entries.

---

# CMD-018 | grep

**Purpose**

Search file contents for lines matching a pattern.

**Syntax**
```bash
grep "Failed" /var/log/auth.log
```

**SOC Use**

Filter logs for relevant events or keywords.

**Important**

A matching line is a lead for investigation, not proof of malicious activity.

---

# CMD-019 | chmod

**Purpose**

Change file or directory permissions.

**Syntax**
```bash
chmod 755 <file>
chmod 644 <file>
chmod +x <file>
chmod u+x <file>
chmod g-w <file>
chmod o-x <file>
```

**SOC Use**

Apply least-privilege permissions and prevent unauthorised modification or execution.

---

# CMD-020 | chown

**Purpose**

Change the owner of a file or directory.

**Syntax**
```bash
sudo chown <owner> <file>
```

**SOC Use**

Assign sensitive files to the appropriate owner.

---

# CMD-021 | chgrp

**Purpose**

Change the group ownership of a file or directory.

**Syntax**
```bash
sudo chgrp <group> <file>
```

**SOC Use**

Assign files to the appropriate team group.

---

# CMD-022 | whoami

**Purpose**

Display the current username.

**Syntax**
```bash
whoami
```

**SOC Use**

Confirm which account is executing commands.

---

# CMD-023 | id

**Purpose**

Display the current user's UID, GID and group memberships.

**Syntax**
```bash
id
```

**SOC Use**

Review account identity and group memberships during access investigations.

---

# CMD-024 | groups

**Purpose**

Display the groups that the current user belongs to.

**Syntax**
```bash
groups
```

**SOC Use**

Check group membership when investigating access and permission issues.

---

# CMD-025 | who

**Purpose**

Display users currently logged into the system.

**Syntax**
```bash
who
```

**SOC Use**

Review active login sessions.

---

# CMD-026 | sudo

**Purpose**

Run a permitted command with elevated privileges.

**Syntax**
```bash
sudo <command>
```

**SOC Use**

Perform administrative tasks with controlled privilege elevation.

**Important**

Use elevated privileges only when required and authorised.

---

# CMD-027 | ps

**Purpose**

Display a snapshot of processes associated with the current session.

**Syntax**
```bash
ps
```

**SOC Use**

Inspect processes in the current terminal session.

---

# CMD-028 | ps aux

**Purpose**

Display a detailed snapshot of system processes.

**Syntax**
```bash
ps aux
```

**SOC Use**

Review process owners, IDs, resource use and command names.

---

# CMD-029 | top

**Purpose**

Display a live, updating view of processes and system resource use.

**Syntax**
```bash
top
```

**SOC Use**

Monitor CPU and memory use and identify processes consuming unusual resources. Press q to exit.

---

# CMD-030 | kill

**Purpose**

Send a signal to a process identified by its PID.

**Syntax**
```bash
kill <PID>
```

**SOC Use**

Request process termination when justified during administration or incident response.

**Important**

The default signal is SIGTERM (15), which requests graceful termination.

---

# CMD-031 | killall

**Purpose**

Send a signal to processes matching a name.

**Syntax**
```bash
killall <process_name>
```

**SOC Use**

Terminate processes by name when appropriate.

**Important**

Use carefully because more than one process may match the name.

---

# CMD-032 | systemctl status

**Purpose**

Display the status of a systemd service.

**Syntax**
```bash
systemctl status <service>
```

**SOC Use**

Check whether a service is active and inspect its status information.

---

# CMD-033 | systemctl list-units

**Purpose**

List loaded systemd units; the example filters the list to services.

**Syntax**
```bash
systemctl list-units --type=service
```

**SOC Use**

Review services currently managed by systemd.

---

# CMD-034 | systemctl start

**Purpose**

Start a service immediately.

**Syntax**
```bash
sudo systemctl start <service>
```

**SOC Use**

Start an approved service when required.

---

# CMD-035 | systemctl stop

**Purpose**

Stop a running service.

**Syntax**
```bash
sudo systemctl stop <service>
```

**SOC Use**

Stop a service when a validated operational or security need exists.

**Important**

Stopping a critical service can disrupt the system; investigate before taking action.

---

# CMD-036 | systemctl restart

**Purpose**

Restart a service.

**Syntax**
```bash
sudo systemctl restart <service>
```

**SOC Use**

Apply service restarts after approved configuration changes.

---

# CMD-037 | systemctl enable

**Purpose**

Configure a service to start automatically at boot.

**Syntax**
```bash
sudo systemctl enable <service>
```

**SOC Use**

Review and manage expected boot-time services.

---

# CMD-038 | systemctl disable

**Purpose**

Prevent a service from starting automatically at boot.

**Syntax**
```bash
sudo systemctl disable <service>
```

**SOC Use**

Review and manage unnecessary boot-time services.

**Important**

Disabling a service does not necessarily stop it immediately.

---

# CMD-039 | journalctl

**Purpose**

Display entries from the systemd journal.

**Syntax**
```bash
journalctl
```

**SOC Use**

Review system events during troubleshooting and investigations.

---

# CMD-040 | journalctl -n

**Purpose**

Display the most recent journal entries.

**Syntax**
```bash
journalctl -n 20
```

**SOC Use**

Quickly review recent system activity.

---

# CMD-041 | journalctl -b

**Purpose**

Display journal entries from the current boot.

**Syntax**
```bash
journalctl -b
```

**SOC Use**

Investigate events that occurred during the current system session.

---

# CMD-042 | journalctl -u

**Purpose**

Display journal entries for a specified systemd unit.

**Syntax**
```bash
journalctl -u ssh
```

**SOC Use**

Investigate activity and errors related to a service.

---

# CMD-043 | hostname -I

**Purpose**

Display IP addresses assigned to the machine.

**Syntax**
```bash
hostname -I
```

**SOC Use**

Quickly identify network addresses assigned to the system.

---

# CMD-044 | ip addr

**Purpose**

Display network interfaces and their assigned IP addresses.

**Syntax**
```bash
ip addr
```

**SOC Use**

Inspect network configuration and interface status.

---

# CMD-045 | ip route

**Purpose**

Display the Linux routing table.

**Syntax**
```bash
ip route
```

**SOC Use**

Identify the default gateway and routes used by the system.

---

# CMD-046 | ping

**Purpose**

Test network reachability using ICMP Echo Requests.

**Syntax**
```bash
ping -c 4 1.1.1.1
```

**SOC Use**

Perform basic connectivity checks.

**Important**

A failed ping does not necessarily mean the destination is offline; ICMP may be filtered.

---

# CMD-047 | getent hosts

**Purpose**

Resolve a hostname using the system's configured name-resolution mechanism.

**Syntax**
```bash
getent hosts example.com
```

**SOC Use**

Check how the operating system resolves domain names.

---

# CMD-048 | nslookup

**Purpose**

Query DNS and display resolver responses.

**Syntax**
```bash
nslookup example.com
```

**SOC Use**

Investigate domain-name resolution.

---

# CMD-049 | dig

**Purpose**

Query DNS servers and inspect DNS responses.

**Syntax**
```bash
dig example.com
dig A example.com +short
```

**SOC Use**

Inspect DNS records when investigating domain resolution.

---

# CMD-050 | ss

**Purpose**

Display socket information, including listening TCP and UDP sockets.

**Syntax**
```bash
ss -tuln
sudo ss -tulpn
```

**SOC Use**

Identify listening ports and, when available, associated processes.

---

# CMD-051 | curl

**Purpose**

Transfer data to or from servers using supported protocols such as HTTP and HTTPS.

**Syntax**
```bash
curl -I https://example.com
curl -I --max-time 10 https://example.com
```

**SOC Use**

Inspect HTTP response headers and test web-server communication.

**Important**

-I sends a HEAD request. A server may not support HEAD even when the website is reachable.

---

# CMD-052 | apt update

**Purpose**

Refresh local package information from configured software repositories.

**Syntax**
```bash
sudo apt update
```

**SOC Use**

Refresh package information before checking for available software and security updates.

**Important**

This command does not upgrade installed packages.

---

# CMD-053 | apt upgrade

**Purpose**

Upgrade installed packages to their available newer versions.

**Syntax**
```bash
sudo apt upgrade
```

**SOC Use**

Apply approved software and security updates.

**Important**

Review proposed changes before confirming the upgrade.

---

# CMD-054 | apt search

**Purpose**

Search configured repositories for available software packages.

**Syntax**
```bash
apt search nginx
```

**SOC Use**

Find software packages when investigating or preparing to install applications.

---

# CMD-055 | apt show

**Purpose**

Display detailed information about a software package.

**Syntax**
```bash
apt show nginx
```

**SOC Use**

Inspect package descriptions, versions and dependencies before installation.

---

# CMD-056 | apt install

**Purpose**

Install software packages from configured repositories.

**Syntax**
```bash
sudo apt install nginx
```

**SOC Use**

Install approved software and security tools.

**Important**

Use trusted repositories and review proposed installation changes.

---

# CMD-057 | apt remove

**Purpose**

Remove an installed software package while generally retaining package-managed configuration files.

**Syntax**
```bash
sudo apt remove nginx
```

**SOC Use**

Remove unnecessary or unauthorised software.

**Important**

Review the removal plan because dependent packages may also be affected.

---

# CMD-058 | apt purge

**Purpose**

Remove an installed package along with its package-managed configuration files.

**Syntax**
```bash
sudo apt purge nginx
```

**SOC Use**

Remove unwanted software and its package-managed configuration files.

**Important**

This does not necessarily remove every user-created file associated with the application.

---

# CMD-059 | apt list --installed

**Purpose**

Display packages currently installed on the system.

**Syntax**
```bash
apt list --installed
```

**SOC Use**

Identify installed software during system inventory and security investigations.

---

# CMD-060 | apt list --upgradable

**Purpose**

Display installed packages that have newer versions available.

**Syntax**
```bash
apt list --upgradable
```

**SOC Use**

Identify software that may require updates, including security patches.

**Important**

Refresh package information with sudo apt update first.

---

# CMD-061 | dpkg -l

**Purpose**

List installed packages and their package-management status.

**Syntax**
```bash
dpkg -l
dpkg -l nginx
```

**SOC Use**

Inspect installed software and check whether a particular package is installed.

---

# CMD-062 | apt-cache policy

**Purpose**

Display package version information, including installed and candidate versions and repository sources.

**Syntax**
```bash
apt-cache policy nginx
```

**SOC Use**

Inspect package versions and repository origins during software security investigations.

---

# CMD-063 | apt-get -s

**Purpose**

Simulate package-management operations without applying the changes.

**Syntax**
```bash
sudo apt-get -s install nginx
sudo apt-get -s upgrade
sudo apt-get -s remove nginx
```

**SOC Use**

Preview proposed package changes before applying them to a system.

**Important**

The -s option performs a simulation; it does not apply the requested package changes.

---

# CMD-064 | apt autoremove

**Purpose**

Remove packages that were automatically installed as dependencies and are no longer required.

**Syntax**
```bash
sudo apt autoremove
```

**SOC Use**

Clean up unused dependencies during system maintenance.

**Important**

Review the proposed package removals before confirming.
