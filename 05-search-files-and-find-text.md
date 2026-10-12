---
title: "Search Files and Find Text"
post: 05
scheduled_date: 2026-10-21
scheduled_day: Wednesday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Search Files and Find Text

**Planned LinkedIn date:** Wednesday, October 21, 2026  
**Series:** Linux Learning Journey — Post 05 of 20  
**Level:** Beginner  
**Topic:** Search and logs

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

🔎 **Linux Learning Journey — Post 05: Search Files and Find Text**

When an app has a problem, we often search its log for a useful message.

### Create a sample log
```bash
mkdir -p ~/linux-lab
cd ~/linux-lab
printf "INFO: Started\nERROR: Timeout\nINFO: Ready\nERROR: Connection failed\n" > app.log
```

### Search it
```bash
grep "ERROR" app.log
grep -n "ERROR" app.log
find . -type f -name "*.log"
grep "ERROR" app.log | wc -l
cut -d ':' -f 1 app.log
```

### What do they do?
- `grep` searches for matching text.
- `grep -n` also shows line numbers.
- `find` searches for files.
- `wc -l` counts lines.
- `cut` extracts a part of each line.

**Expected result:** The error count is `2`. The file path shown by `find` depends on your current folder.

🧪 **Practice:** Change the log text and count the errors again.

💡 **DevOps connection:** Searching logs is a basic troubleshooting skill.

#Linux #LogAnalysis #LinuxCommands #DevOps #Killercoda #CloudEngineering
