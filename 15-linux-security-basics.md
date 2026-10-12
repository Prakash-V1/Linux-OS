---
title: "Linux Security Basics"
post: 15
scheduled_date: 2026-11-13
scheduled_day: Friday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Linux Security Basics

**Planned LinkedIn date:** Friday, November 13, 2026  
**Series:** Linux Learning Journey — Post 15 of 20  
**Level:** Beginner  
**Topic:** Security

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

🛡️ **Linux Learning Journey — Post 15: Linux Security Basics**

Good security starts with knowing who you are, what you can access, and which services are listening.

### Commands to practice
```bash
whoami
id
ls -l ~/linux-lab
stat ~/linux-lab/app.log
sudo -l
ss -lnt
last
```

Some commands may show limited information or need extra permissions in a container.

### What I learned
- `id` shows user and group IDs.
- `ls -l` shows ownership and permissions.
- `stat` displays file details.
- `sudo -l` shows which commands your account may run with sudo.
- `ss -lnt` lists listening TCP sockets.
- `last` reads available login records.

🧪 **Practice:** Check the permissions of a file you created. Decide what access the owner, group, and others need.

💡 **DevOps connection:** Least privilege helps protect application data and infrastructure.

#LinuxSecurity #CyberSecurity #DevOps #CloudSecurity #Killercoda #LinuxLearning
