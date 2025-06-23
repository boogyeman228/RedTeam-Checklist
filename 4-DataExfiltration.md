# Data Exfiltration
###  Goal: Extract sensitive information from the target environment without detection.

# Techniques:
- `Compress and encrypt data before exfil`
- `Use staging via SMB, FTP, or shared drives`
- `HTTP/S, DNS, or cloud service tunnels`
- `Chunked upload over long intervals to avoid triggering alerts`

# Tools:
- scp, rsync, curl, wget
rclone (supports Dropbox, Google Drive, etc.)

dnscat2, iodine, dns2tcp

netcat, smbclient

Noise level:
DNS tunneling: 🔇 Silent (if slow)

HTTPS upload: ⚠️ Medium

FTP, SCP: 🔊 Loud

Notes:
Use AES or GPG to encrypt before uploading.

Don’t exfil full disks—target sensitive directories: Documents, Desktop, config folders.

Obfuscate filenames (e.g., project_Q2.zip instead of passwords.zip).
