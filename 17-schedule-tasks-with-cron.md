---
title: "Schedule Tasks with Cron"
post: 17
scheduled_date: 2026-11-18
scheduled_day: Wednesday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Schedule Tasks with Cron

**Planned LinkedIn date:** Wednesday, November 18, 2026  
**Series:** Linux Learning Journey — Post 17 of 20  
**Level:** Beginner  
**Topic:** Scheduling

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

⏰ **Linux Learning Journey — Post 17: Schedule Tasks with Cron**

Cron can run a command at a planned time. It is often used for recurring checks and maintenance.

### Inspect your setup
```bash
date
crontab -l
```

Example schedule:
```cron
0 9 * * * /bin/bash /home/student/linux-lab/disk-check.sh >> /home/student/linux-lab/disk-check.log 2>&1
```

This runs every day at 9:00 AM in the scheduler's timezone. Replace `/home/student` with the real absolute path for your lab user.

### Understand `0 9 * * *`
- Minute: `0`
- Hour: `9`
- Day of month: `*` (every day)
- Month: `*` (every month)
- Day of week: `*` (every day)

`>>` appends output to a log file. `2>&1` sends error output to the same place.

🧪 **Practice:** Explain the schedule and inspect your current crontab. The example is not installed by the commands above.

💡 **DevOps connection:** Scheduled jobs can run health checks, create reports, and automate routine work.

#Linux #Cron #BashScripting #DevOps #Automation #Killercoda
