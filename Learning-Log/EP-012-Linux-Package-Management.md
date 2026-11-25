EP-012

*Date:* 25 November 2026
*Topic:* Linux Package Management & Software Security

*Topics learned:*
- Linux packages and package managers.
- APT and DPKG.
- Software repositories and package dependencies.
- Refreshing package information versus upgrading installed software.
- Searching for and inspecting packages.
- Checking installed packages and available upgrades.
- Inspecting package versions and repository sources.
- Installing, removing and purging packages.
- Simulating package operations before applying changes.
- **Linux commands learned:** `apt update`, `apt upgrade`, `apt search`, `apt show`, `apt install`, `apt remove`, `apt purge`, `apt autoremove`, `apt list --installed`, `apt list --upgradable`, `dpkg -l`, `apt-cache policy`, `apt-get -s`.

*Cybersecurity lesson:* Package management helps analysts identify outdated software, verify package sources and apply approved security updates. Proposed changes should be reviewed before modifying a system.

*Key takeaway:* Refreshing package information is not the same as upgrading software; inspect package sources and proposed changes before proceeding.