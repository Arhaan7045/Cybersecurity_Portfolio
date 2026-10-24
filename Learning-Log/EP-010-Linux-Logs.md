# EP-010 - Linux Logs & journalctl

## Mission

Investigated Linux system logs and learned how security analysts use logs to understand user activity, authentication events, services, and system behavior.

## Commands Learned

- journalctl
- journalctl -n
- journalctl -b
- journalctl -u
- tail
- less
- grep

## Key Concepts

- Linux logs
- /var/log
- systemd journal
- Authentication logs
- Log analysis
- Security events

## Biggest Takeaway

Logs provide evidence of what happened on a system. Security analysts use them to identify patterns and investigate suspicious activity.

## SOC Perspective

A single failed login may not mean much, but repeated authentication failures followed by a successful login can become a significant security event.

## Interview Questions

- Why are logs important in cybersecurity?
- What is journalctl?
- What is the purpose of /var/log?
- What does tail do?
- How can grep help during log analysis?

## Next Lesson

Linux Networking Commands


---

## Practical Evidence and Verification (complete from your actual lab)

> Fill this section only with observations from work you personally performed. Do not invent output or mark a result as passed without checking it.

### Investigation question

- What specific system or log question was I trying to answer?
- Which log source did I inspect, and why was it appropriate?

### Commands actually run

```bash
# Add the exact commands you ran, for example the relevant journalctl query.
```

### Observed result

- **What I observed:**
- **Relevant timestamps/service/event details:**
- **What the output supports:**
- **What it does not establish:**

### Evidence links

- [ ] Link genuine screenshot(s) from `../SS/` using the actual filename.
- [ ] Confirm the screenshot shows the command and enough output to interpret it.
- [ ] Remove secrets or personal information before publishing.

### Analyst reasoning

- Could the observed event have a benign explanation?
- What additional log source or context would I check next?
- What would increase or reduce confidence in a suspicious-activity hypothesis?

### Verification status

- **Status:** Needs verification / Partially verified / Demonstrated
- **Mini challenge attempted:**
- **Result observed:**
- **Remaining gaps:**

### Interview explanation

In my own words, explain why system logs matter, what this specific exercise showed, and why one event alone may not prove an incident.

