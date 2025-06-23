# 📦Persistence
### Goal: Maintain long-term access to the environment even if the initial vector is closed.

## Techniques:
- Registry Run keys or Startup folder backdoors
- Scheduled Tasks or cron jobs
- Creating new users or adding to admin group
- Planting SSH keys or abusing authorized_keys
- WMI subscriptions or DLL hijack
- Golden / Silver Ticket creation

## Tools:
- `chtasks, reg, cron, at`
- `Empire, SharpPersist`
- `Mimikatz, Rubeus`
- `PowerView.ps1`
- `wmic, net user`

## Noise level:
- Registry / autoruns: 🔇 Silent
- Scheduled tasks: ⚠️ Medium
- Golden ticket: 🔊 Loud (if abused heavily)

# Notes:
- Persistence should be layered (multiple methods).
- Avoid crashing services — test persistence before exiting.
- Keep backup access paths (e.g., reverse shell listener + RDP)
