---
title: "Write Your First Bash Script"
post: 16
scheduled_date: 2026-11-16
scheduled_day: Monday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Write Your First Bash Script

**Planned LinkedIn date:** Monday, November 16, 2026  
**Series:** Linux Learning Journey — Post 16 of 20  
**Level:** Beginner  
**Topic:** Bash scripting

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

🤖 **Linux Learning Journey — Post 16: My First Bash Script**

A Bash script saves commands so we can run them together. This helps reduce repeated manual work.

### Create a disk-check script
```bash
mkdir -p ~/linux-lab
cd ~/linux-lab

cat > disk-check.sh <<'EOF'
#!/usr/bin/env bash
set -u

threshold=80
usage=$(df -P "$HOME" | awk 'NR==2 {gsub(/%/, "", $5); print $5}')

if [[ "$usage" =~ ^[0-9]+$ ]]; then
  if (( usage >= threshold )); then
    echo "WARNING: Disk usage is ${usage}%"
  else
    echo "OK: Disk usage is ${usage}%"
  fi
else
  echo "ERROR: Could not read disk usage"
  exit 1
fi
EOF

bash disk-check.sh
```

### What does it teach?
- Variables store values.
- `$(...)` captures command output.
- `if` checks a condition.
- `awk` extracts the disk usage number.
- `exit 1` signals an error.

**Expected result:** The script prints `OK` or `WARNING` based on the filesystem containing your home folder. The percentage varies by lab.

🧪 **Practice:** Change `threshold=80` to `threshold=50` and run the script again.

💡 **DevOps connection:** Scripts can automate checks, deployments, and routine tasks.

#BashScripting #Linux #DevOpsAutomation #CloudEngineering #Killercoda #LearningInPublic
