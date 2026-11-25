EP-009

*Date:* Not recorded
*Topic:* Linux Services & systemd

*Topics learned:*
- Understanding background services and systemd.
- Checking service status and listing loaded service units.
- Starting, stopping and restarting services.
- Enabling and disabling services at system boot.
- Understanding the difference between starting and enabling a service.
- **Linux commands learned:** `systemctl status`, `systemctl list-units`, `systemctl start`, `systemctl stop`, `systemctl restart`, `systemctl enable`, `systemctl disable`.

*Cybersecurity lesson:* Attackers may create or modify services to maintain persistence. Analysts should investigate unfamiliar services and their purpose before stopping or disabling them.

*Key takeaway:* Starting a service affects it now; enabling a service configures it to start automatically at boot.