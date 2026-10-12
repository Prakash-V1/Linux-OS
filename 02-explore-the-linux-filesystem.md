---
title: "Explore the Linux Filesystem"
post: 02
scheduled_date: 2026-10-14
scheduled_day: Wednesday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Explore the Linux Filesystem

**Planned LinkedIn date:** Wednesday, October 14, 2026  
**Series:** Linux Learning Journey — Post 02 of 20  
**Level:** Beginner  
**Topic:** Files and folders

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

📂 **Linux Learning Journey — Post 02: Explore the Linux Filesystem**

Linux files and folders are arranged in a tree. The top directory is `/`, called root.

### Try these commands
```bash
pwd
ls -lah /
cd /etc
pwd
ls
cd /var/log
pwd
cd -
```

### What do they mean?
- `pwd` shows your current directory.
- `ls -lah` lists files, including hidden files, with details.
- `cd` changes the directory.
- `cd -` returns to the previous directory.

### Useful folders
- `/etc` — system configuration
- `/var/log` — many system and app logs
- `/home` — users' home folders
- `/tmp` — temporary files
- `/proc` — information about processes and the kernel

**Expected result:** `pwd` prints a path and `ls` lists folder contents. The exact files depend on your lab.

🧪 **Practice:** Visit `/etc`, `/var/log`, and `/tmp`, then list their contents.

💡 **DevOps connection:** Knowing where logs and configuration live helps when an application has a problem.

#Linux #LinuxCommands #DevOps #CloudEngineering #Killercoda #LearningInPublic
