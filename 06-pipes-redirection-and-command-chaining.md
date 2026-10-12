---
title: "Pipes, Redirection, and Command Chaining"
post: 06
scheduled_date: 2026-10-23
scheduled_day: Friday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Pipes, Redirection, and Command Chaining

**Planned LinkedIn date:** Friday, October 23, 2026  
**Series:** Linux Learning Journey — Post 06 of 20  
**Level:** Beginner  
**Topic:** Command combinations

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

🔗 **Linux Learning Journey — Post 06: Pipes and Redirection**

Commands become more useful when we combine them.

### Try this
```bash
cd ~/linux-lab
grep "ERROR" app.log > errors.txt
cat errors.txt
grep "INFO" app.log >> errors.txt
cat errors.txt
grep "ERROR" app.log | wc -l
mkdir -p reports && echo "Reports directory ready"
```

Check a command's exit status:
```bash
grep "WARNING" app.log
echo $?
```

### Simple explanations
- `>` writes to a file and replaces its old contents.
- `>>` adds output to the end of a file.
- `|` sends one command's output to another command.
- `&&` runs the next command only if the first succeeds.
- `$?` stores the previous command's exit status.

**Expected result:** The error count is `2`. If `WARNING` is not found, `grep` usually returns status `1`.

🧪 **Practice:** Save all error lines to a file and count them.

#Linux #Bash #LinuxCommands #DevOpsAutomation #Killercoda #CloudComputing
