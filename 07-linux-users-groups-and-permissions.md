---
title: "Linux Users, Groups, and Permissions"
post: 07
scheduled_date: 2026-10-26
scheduled_day: Monday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Linux Users, Groups, and Permissions

**Planned LinkedIn date:** Monday, October 26, 2026  
**Series:** Linux Learning Journey — Post 07 of 20  
**Level:** Beginner  
**Topic:** Permissions

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

🔐 **Linux Learning Journey — Post 07: Users, Groups, and Permissions**

Linux permissions decide who can read, change, or run a file.

### Try this
```bash
whoami
id
groups
mkdir -p ~/linux-lab/shared
touch ~/linux-lab/shared/report.txt
chmod 640 ~/linux-lab/shared/report.txt
ls -l ~/linux-lab/shared/report.txt
```

### What does `640` mean?
- Owner: `6` means read and write.
- Group: `4` means read only.
- Others: `0` means no permissions.

**Expected result:** `ls -l` commonly shows `-rw-r-----` for this file.

🧪 **Practice:** Try `chmod 600` on your test file and compare the permissions.

💡 **DevOps connection:** Correct permissions help protect configuration files and application data.

⚠️ Only change permissions on files you created for practice.

#LinuxSecurity #LinuxPermissions #DevOps #CloudSecurity #Killercoda #LinuxLearning
