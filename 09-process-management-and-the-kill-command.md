---
title: "Process Management and the kill Command"
post: 09
scheduled_date: 2026-10-30
scheduled_day: Friday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Process Management and the kill Command

**Planned LinkedIn date:** Friday, October 30, 2026  
**Series:** Linux Learning Journey — Post 09 of 20  
**Level:** Beginner  
**Topic:** Processes

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

⚙️ **Linux Learning Journey — Post 09: Process Management**

A process is a running program. Linux has commands to inspect and manage processes.

### Start a test process
```bash
sleep 300 &
pgrep -a -x sleep
ps aux | head
```

Find the PID of the `sleep 300` process you started, then replace `PID_NUMBER` below with that number:
```bash
kill -TERM PID_NUMBER
```

Verify:
```bash
pgrep -a -x sleep
```

### Key points
- `ps` lists process information.
- `pgrep` finds processes by name or pattern.
- `top` shows a live process view.
- `kill -TERM` asks a process to stop gracefully.
- `kill -KILL` forces a process to stop and should be a last resort.

**Expected result:** Your test process should disappear after it exits. If other `sleep` processes exist, do not stop them.

🧪 **Practice:** Start and stop only the process you created.

💡 **DevOps connection:** Process knowledge helps investigate apps that hang or use too much CPU.

#Linux #ProcessManagement #DevOps #Killercoda #Troubleshooting #LinuxCommands
