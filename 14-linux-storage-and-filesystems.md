---
title: "Linux Storage and Filesystems"
post: 14
scheduled_date: 2026-11-11
scheduled_day: Wednesday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Linux Storage and Filesystems

**Planned LinkedIn date:** Wednesday, November 11, 2026  
**Series:** Linux Learning Journey — Post 14 of 20  
**Level:** Beginner  
**Topic:** Storage

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

💽 **Linux Learning Journey — Post 14: Storage and Filesystems**

A full disk can stop an app from writing files or logs. Today, I’m practicing safe storage checks.

### Commands
```bash
lsblk
df -h
df -i
findmnt
du -sh ~/linux-lab
```

If available:
```bash
blkid
```

### What do they show?
- `lsblk` lists block devices.
- `df -h` shows filesystem capacity and free space.
- `df -i` shows inode usage.
- `findmnt` lists mounted filesystems.
- `du -sh` estimates a directory's size.
- `blkid` reports filesystem identifiers and types.

**Expected result:** Commands show the devices and filesystems visible to your lab. A container may show limited information.

🧪 **Practice:** Compare filesystem usage with the size of your lab directory.

⚠️ This is an inspection exercise. Do not format or repartition disks in a beginner lab.

#LinuxStorage #LinuxAdministration #DevOps #CloudInfrastructure #Killercoda #Troubleshooting
