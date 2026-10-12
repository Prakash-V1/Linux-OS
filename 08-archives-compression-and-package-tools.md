---
title: "Archives, Compression, and Package Tools"
post: 08
scheduled_date: 2026-10-28
scheduled_day: Wednesday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Archives, Compression, and Package Tools

**Planned LinkedIn date:** Wednesday, October 28, 2026  
**Series:** Linux Learning Journey — Post 08 of 20  
**Level:** Beginner  
**Topic:** Archives and packages

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

📦 **Linux Learning Journey — Post 08: Archives and Package Tools**

Linux administrators often package files for backup or transfer. They also use package managers to install software.

### Create and inspect an archive
```bash
mkdir -p ~/linux-lab/project
echo "Sample application" > ~/linux-lab/project/app.txt
tar -czf ~/linux-lab/project.tar.gz -C ~/linux-lab/project .
tar -tzf ~/linux-lab/project.tar.gz
file ~/linux-lab/project.tar.gz
```

### Package tools depend on the distribution
```bash
# Debian / Ubuntu: list installed packages
apt list --installed

# Fedora / RHEL-family: query installed RPM packages
rpm -qa
```

### Remember
- `tar` groups files into an archive.
- `-z` uses gzip compression.
- `tar -t` lists archive contents.
- `apt` is common on Debian/Ubuntu.
- `dnf` is common on Fedora and many RHEL-family systems.
- `rpm` queries RPM package information.

**Expected result:** The archive listing includes `app.txt`. Package commands work only on compatible systems.

🧪 **Practice:** Create an archive and list its contents.

#Linux #PackageManagement #DevOps #CloudEngineering #Killercoda #LinuxAdministration
