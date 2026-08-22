# EP-009 - Linux Services

## Mission

Investigated how Linux background services work and how analysts can check their status and startup configuration.

## Commands Learned

- systemctl status
- systemctl list-units
- systemctl start
- systemctl stop
- systemctl restart
- systemctl enable
- systemctl disable

## Key Concepts

- Linux services
- systemd
- systemctl
- Service status
- Service startup
- Boot-time services

## Biggest Takeaway

A service is a background system function. Security analysts should investigate unknown services instead of immediately assuming they are malicious.

## SOC Perspective

Attackers may create or modify services to maintain persistence on a compromised Linux system.

## Interview Questions

- What is a Linux service?
- What is systemd?
- Difference between start and enable?
- How do you check whether a service is running?
- Why shouldn't you immediately stop an unknown service?

## Next Episode

Linux Logs & Journalctl