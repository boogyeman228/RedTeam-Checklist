# 🔊 Technique Noise Levels & Detection Tips

## 🔓 Initial Access

| Technique            | Noise Level | Detection Tip                            | Evasion Suggestion                      |
|----------------------|-------------|------------------------------------------|-----------------------------------------|
| Phishing (macro)     | 🔇 Silent    | Office macro execution                   | Obfuscate VBA, use signed docs          |
| Responder poisoning  | 🔊 Loud      | LLMNR/NBT-NS flood, NBNS probes          | Run briefly, use isolated subnet        |
| Public exploit (CVE) | ⚠️ Medium   | Version probing & payload drop           | Use proxychains, spoofed user-agents    |

## 🔼 Privilege Escalation

| Technique             | Noise Level | Detection Tip                            | Evasion Suggestion                      |
|-----------------------|-------------|------------------------------------------|-----------------------------------------|
| Mimikatz LSASS dump   | 🔊 Loud      | LSASS memory access                      | Use `sekurlsa::logonpasswords` stealth mode |
| LinPEAS / WinPEAS     | ⚠️ Medium   | File enumeration, service probing        | Transfer locally, rename executable     |

...

## 🔁 Lateral Movement

| Technique             | Noise Level | Detection Tip                            | Evasion Suggestion                      |
|-----------------------|-------------|------------------------------------------|-----------------------------------------|
| CrackMapExec          | 🔊 Loud      | Mass authentication attempts             | Limit targets, increase delay           |
| Pass-the-Hash         | ⚠️ Medium   | NTLM auth logs                           | Use new hashes per target               |
