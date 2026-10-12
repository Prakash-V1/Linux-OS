---
title: "Linux Interview Questions and What I Learned"
post: 20
scheduled_date: 2026-11-25
scheduled_day: Wednesday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Linux Interview Questions and What I Learned

**Planned LinkedIn date:** Wednesday, November 25, 2026  
**Series:** Linux Learning Journey — Post 20 of 20  
**Level:** Beginner  
**Topic:** Interview preparation

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

🎓 **Linux Learning Journey — Post 20: Linux Interview Questions**

I’ve reached the final post in my planned 20-post Linux learning series!

The goal was not only to remember commands, but also to understand how to use them.

### 7 questions to practice

**1. What is the difference between SIGTERM and SIGKILL?**  
`SIGTERM` asks a process to stop gracefully. `SIGKILL` forces it to stop and cannot be handled by the process.

**2. How do you investigate a failed service?**  
Check `systemctl status`, read relevant `journalctl` logs, find the cause, and verify recovery.

**3. What is the difference between `df` and `du`?**  
`df` shows filesystem usage. `du` estimates space used by files and folders.

**4. How do Linux permissions work?**  
They control read, write, and execute access for the owner, group, and others.

**5. How do you check whether a port is listening?**  
Use `ss -lnt` and inspect the app service and logs.

**6. How can you schedule a script?**  
Cron can run recurring tasks when the scheduler is installed and configured.

**7. What do you do when a disk is full?**  
Check `df -h` and `df -i`, find large folders with `du`, and investigate before removing anything.

🧪 **Final challenge:** Answer each question in your own words and demonstrate a command in your lab.

Thank you for following this learning journey. Next, I plan to apply these foundations to more DevOps and Cloud projects.

💬 What Linux topic should I learn next?

#Linux #LinuxInterviewQuestions #DevOps #CloudComputing #LinuxAdministration #Killercoda #LearningInPublic
