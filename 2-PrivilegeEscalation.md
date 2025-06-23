# Privilege Escalation
Goal: To increase privileges from a regular user to an administrator

## Techniques:
SUID/SGID binary abuse (find / -perm -4000)
Kernel exploits (e.g. DirtyCow, DirtyPipe, PrintNightmare)
Misconfigured sudo permissions (sudo -l)
Exploiting writable services / timers / cron jobs
DLL hijacking (Windows)
Password reuse / token impersonation (mimikatz, Rubeus)
Insecure PATH environment variable manipulation

## Tools:
linPEAS / winPEAS
sudo -l
GTFOBins
linux-exploit-suggester.sh
PowerUp.ps1
mimikatz
Rubeus

## Noise level:
Enumeration tools: 🔇 Silent
Exploits / LSASS dump: 🔊 Loud
Sudo or SUID abuse: ⚠️ Medium

#Notes:
Always run enumeration tools first.
Kernel exploits may crash the system—use as last resort.
Look for writable scripts in cron, systemd, or user-controlled binaries.
