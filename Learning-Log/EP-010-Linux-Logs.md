EP-010

*Date:* Not recorded
*Topic:* Linux Logs & journalctl

*Topics learned:*
- The purpose of Linux system and authentication logs.
- The `/var/log` directory and the systemd journal.
- Viewing recent journal entries.
- Filtering journal entries by boot and service.
- Reviewing log files and searching for relevant events.
- **Linux commands learned:** `journalctl`, `journalctl -n`, `journalctl -b`, `journalctl -u`, `tail`, `less`, `grep`.

*Cybersecurity lesson:* Logs provide evidence of system and user activity. Repeated authentication failures followed by a successful login may deserve investigation, but a single failed login does not by itself prove an attack.

*Key takeaway:* Interpret log events with timestamps and surrounding context rather than judging an incident from one entry.