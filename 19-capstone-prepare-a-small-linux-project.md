---
title: "Capstone: Prepare a Small Linux Project"
post: 19
scheduled_date: 2026-11-23
scheduled_day: Monday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Capstone: Prepare a Small Linux Project

**Planned LinkedIn date:** Monday, November 23, 2026  
**Series:** Linux Learning Journey — Post 19 of 20  
**Level:** Beginner  
**Topic:** Capstone

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

🚀 **Linux Learning Journey — Post 19: My Linux Hands-on Project**

It’s time to combine several Linux skills in one small project.

### 1. Create project folders
```bash
mkdir -p ~/linux-project/{app,logs,backup}
```

### 2. Add sample log messages
```bash
echo "Application started" > ~/linux-project/logs/app.log
echo "ERROR: Simulated failure" >> ~/linux-project/logs/app.log
```

### 3. Inspect the project
```bash
ls -lah ~/linux-project
grep -n "ERROR" ~/linux-project/logs/app.log
df -h
free -h
ps aux | head
```

### 4. Create a backup archive
```bash
tar -czf ~/linux-project/backup/logs.tar.gz -C ~/linux-project logs
tar -tzf ~/linux-project/backup/logs.tar.gz
```

**Expected result:** The error search finds the simulated error. The archive listing includes `logs/app.log`.

🧪 **Practice challenge:** Explain how you would investigate the error, preserve the logs, and verify that the app recovered.

💡 **Key takeaway:** Linux skills are more useful when we combine commands into a clear workflow.

This is a local practice project; it does not deploy a real cloud application.

#Linux #DevOpsProject #CloudEngineering #BashScripting #Killercoda #LearningInPublic
