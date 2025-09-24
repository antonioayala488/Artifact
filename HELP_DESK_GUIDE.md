# 📘 Help Desk Troubleshooting Guide

*A practical guide for Tier 1 / Tier 2 IT support staff to quickly resolve common issues in small and medium-sized organizations.*

---

## 📑 Table of Contents

1. [Password Reset Issues](#1-password-reset-issues)
2. [VPN Connection Failure](#2-vpn-connection-failure)
3. [Printer Not Responding](#3-printer-not-responding)
4. [Slow Computer Performance](#4-slow-computer-performance)
5. [Email Delivery Problems](#5-email-delivery-problems)
6. [Appendix: Quick Reference Table](#-appendix-quick-reference-table)

---

## 1. Password Reset Issues

**Symptoms:**

* User forgot their password
* Account is locked after too many attempts

**Resolution Steps:**

1. Verify user identity (employee ID or security questions).
2. In Active Directory:

   * Right-click user → *Reset Password*.
   * Ensure “User must change password at next login” is checked.
3. If using cloud services (e.g., Microsoft 365):

   * Use Admin Portal → Users → Reset Password.
4. Document the reset in the ticket.

**Preventive Tip:** Encourage use of self-service password reset (SSPR) if enabled.

---

## 2. VPN Connection Failure

**Symptoms:**

* User cannot connect to VPN
* Error: “Authentication failed” or “Cannot reach server”

**Resolution Steps:**

1. Verify network connection (Wi-Fi / Ethernet).
2. Ping VPN server to confirm it’s reachable.
3. Check user’s VPN credentials are active.
4. Reset VPN profile (delete + re-add).
5. If issue persists → escalate to Network Admin.

**Preventive Tip:** Provide a quick-start guide for VPN installation.

---

## 3. Printer Not Responding

**Symptoms:**

* User cannot print
* Jobs stuck in queue

**Resolution Steps:**

1. Confirm printer is powered on and connected to network.
2. Clear print queue:

   * Windows: `services.msc` → Restart *Print Spooler*
   * macOS: Clear via *System Preferences → Printers*.
3. Test with a small document.
4. If multiple users affected → check shared printer server.

**Preventive Tip:** Schedule weekly checks of print queues.

---

## 4. Slow Computer Performance

**Symptoms:**

* User reports lag or freezing
* High CPU or memory usage

**Resolution Steps:**

1. Check Task Manager (Windows) / Activity Monitor (Mac).
2. Close unnecessary background processes.
3. Run disk cleanup (Windows: `cleanmgr`).
4. Ensure system updates and drivers are current.
5. Run antivirus scan.

**Preventive Tip:** Set policies for auto-updates and patching.

---

## 5. Email Delivery Problems

**Symptoms:**

* User not receiving emails
* Emails stuck in outbox

**Resolution Steps:**

1. Verify network connection.
2. Check Outlook / client is online.
3. Ensure mailbox is not full.
4. Verify mail server status (e.g., Exchange, O365).
5. Send test email internally and externally.
6. If unresolved → escalate to Exchange/O365 Admin.

**Preventive Tip:** Educate users on mailbox management and phishing awareness.

---

# 📊 Appendix: Quick Reference Table

| Issue               | Quick Fix                      | Escalate To     |
| ------------------- | ------------------------------ | --------------- |
| Password Reset      | Reset via AD / 365 Admin       | Security Admin  |
| VPN Failure         | Check network + re-add profile | Network Admin   |
| Printer Not Working | Restart spooler + test print   | Systems Admin   |
| Slow PC             | Close tasks + update system    | Desktop Support |
| Email Issues        | Check mailbox + server status  | Mail Admin      |

