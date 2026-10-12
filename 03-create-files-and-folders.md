---
title: "Create Files and Folders"
post: 03
scheduled_date: 2026-10-16
scheduled_day: Friday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Create Files and Folders

**Planned LinkedIn date:** Friday, October 16, 2026  
**Series:** Linux Learning Journey — Post 03 of 20  
**Level:** Beginner  
**Topic:** File basics

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

⌨️ **Linux Learning Journey — Post 03: Create Files and Folders**

Today I’m practicing commands used by Linux users and administrators.

### Try it
```bash
mkdir -p ~/linux-lab/logs
cd ~/linux-lab
touch app.log
echo "Linux practice started" > app.log
ls -lah
file app.log
stat app.log
```

### Simple explanations
- `mkdir -p` creates folders and missing parent folders.
- `touch` creates an empty file if it does not exist.
- `echo` prints text.
- `>` writes output to a file, replacing its old contents.
- `file` reports a file type.
- `stat` shows file details.

**Expected result:** `ls` lists `app.log`; `file` will usually identify it as a text file.

🧪 **Practice:** Create `project`, `logs`, and `backup` folders and add a sample file.

⚠️ Remember: `>` can overwrite a file. Use it only with practice files.

#Linux #LinuxCommands #DevOps #CloudComputing #Killercoda #LearningInPublic
