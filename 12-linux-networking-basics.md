---
title: "Linux Networking Basics"
post: 12
scheduled_date: 2026-11-06
scheduled_day: Friday
status: draft
platform: LinkedIn
practice_platform: Killercoda
---

# Linux Networking Basics

**Planned LinkedIn date:** Friday, November 6, 2026  
**Series:** Linux Learning Journey — Post 12 of 20  
**Level:** Beginner  
**Topic:** Networking

> **Status: Draft only.** This file does not publish or schedule anything on LinkedIn.

---

🌐 **Linux Learning Journey — Post 12: Linux Networking Basics**

When an app cannot connect, check the network step by step.

### Try these commands
```bash
ip addr
ip route
ss -lnt
getent hosts example.com
curl -I https://example.com
ping -c 4 127.0.0.1
```

### Simple explanations
- `ip addr` shows network interfaces and addresses.
- `ip route` shows routing information.
- `ss -lnt` lists listening TCP sockets.
- `getent hosts` checks name lookup using system settings.
- `curl -I` requests HTTP headers.
- `ping` tests ICMP reachability when permitted.

**Expected result:** Interface and route commands show local configuration. Internet tests may fail if the lab blocks outbound access.

🧪 **Practice:** Check an address, route, and listening port. If internet access is blocked, use a lab-provided endpoint.

💡 **DevOps connection:** These commands help investigate DNS, connectivity, and port problems.

#LinuxNetworking #DevOps #CloudNetworking #Killercoda #Troubleshooting #LinuxCommands
