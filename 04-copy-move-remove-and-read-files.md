---
title: "Copy, Move, Remove, and Read Files"
post: 04
scheduled_date: 2026-10-19
scheduled_day: Monday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Copy, Move, Remove, and Read Files

**Planned LinkedIn date:** Monday, October 19, 2026  
**Series:** Linux Learning Journey — Post 04 of 20  
**Level:** Beginner  
**Topic:** File operations

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

📄 **Linux Learning Journey — Post 04: Work with Files**

Linux has commands to copy, rename, remove, and read files.

### Practice
```bash
mkdir -p ~/linux-lab
cd ~/linux-lab
printf "INFO: App started\nERROR: Test failure\n" > app.log
cp app.log app-copy.log
mv app-copy.log archive.log
head -n 5 app.log
tail -n 5 app.log
cat app.log
```

Remove only the practice copy after checking it:
```bash
rm archive.log
```

### Remember
- `cp` copies a file.
- `mv` moves or renames a file.
- `rm` removes a file.
- `head` shows the first lines.
- `tail` shows the last lines.
- `cat` prints the file contents.

**Expected result:** `cat app.log` shows an INFO line and an ERROR line.

🧪 **Practice:** Copy a file, rename the copy, and check with `ls`.

⚠️ Check the target before using `rm`. Do not delete files you do not recognize.

#Linux #LinuxAdministration #DevOps #Troubleshooting #Killercoda #LinuxLearning
