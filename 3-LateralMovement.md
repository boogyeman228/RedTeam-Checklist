# Lateral Movement
### Goal: To spread across the network and compromise other machines or domain accounts

## Techniques:
- Pass-the-Hash / Pass-the-Ticket
- SMB and WMI command execution
- PowerShell Remoting / WinRM
- PsExec or Impacket scripts (smbexec, wmiexec, etc.)
- RDP lateral access
- Kerberoasting / delegation abuse

## Tools:
- `CrackMapExec`
- `evil-winrm`
- `Impacket toolkit`
- `Rubeus`
- `BloodHound`
- `SharpHound`
- `PSExec`

## Noise level:
- PsExec, RDP, WMI: 🔊 Loud
- Kerberos attacks (tickets): ⚠️ Medium
- Token impersonation: 🔇 Silent (if done right)

## Notes:
- Prefer stealthy token-based movement over noisy RDP/PsExec.
- Use BloodHound to identify high-value paths before moving.
- Disable telemetry when possible.
