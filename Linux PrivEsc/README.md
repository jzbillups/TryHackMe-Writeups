# Linux PrivEsc: Methodologies & Tools

**Platform:** TryHackMe | **Category:** Linux / Privilege Escalation | **Date:** July 2026 | **Link:** https://tryhackme.com/room/linprivesc |

## 1. Executive Summary
This project explores standard privilege escalation methodologies within a Linux environment. The objective was to utilize automated enumeration scripts alongside manual techniques to identify system misconfigurations, vulnerable binaries, and weak file permissions to escalate from a low-privileged user to root.

**Tools Deployed:**
* **SSH:** Initial access and remote command execution.
* **LinEnum / LinPEAS:** Automated enumeration scripts to identify privilege escalation vectors.
* **GTFOBins:** Curated resource for exploiting native Unix binaries to bypass security restrictions.
* **Native Linux Commands:** Built-in utilities (`find`, `sudo`, `tar`) used for manual enumeration and exploitation.

---

## 2. Initial Access & System Enumeration
**Objective:** Establish a foothold on the target machine and gather a baseline of system information to identify potential attack paths.

### 2.1 Initialization
I first accessed the target machine via SSH using the low-privileged credentials provided for the initial user.
```bash
ssh user@$box
