# 🔓 Initial Access
###  Goal: Gain the first foothold into the target network by compromising a user, system, or exposed service.

## Techniques:
- Phishing (macro, link)
- LLMNR/NBT-NS poisoning (Responder)
- Malicious document (.docx, .lnk, .iso)
- Exploiting public-facing apps
- USB HID attacks (Rubber Ducky/Flipper)

## Tools:
- `msfvenom`
- `responder`
- `evil-winrm`
- `Nishang`

## Noise level:
- Phishing: 🔇 Quiet (if without AV detect)
- Responder: 🔊 Loud (spam at network)
- Public Exploit: ⚠️ Medium-High

## Notes:
- Always check if AV/EDR is in place.
- Use base64 encoding or DNS tunnel to avoid detection.
