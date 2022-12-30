# SYNOPSIS
This script was created while completing the blind ssrf module of AWAE. Given a CIDR (Classless Inter-Domain Routing) format network address, generate all valid IPv4 addresses in that range.
## NOTES
- Version:        1.0
- Author:         Zinhart
- Purpose: Created while studying for OSWE certification
- Inspired by: https://github.com/EliteLoser/PSipcalc/blob/master/PSipcalc.ps1 
## Examples
Piping
```powershell
'172.16.0.0/24' | ./Convert-CIDRInfo.ps1
```
Enumerating Gateways
```powershell
./Convert-CIDRInfo.ps1 -NetworkAddress '172.16.0.0/12' -Gateway
```
Enumerating IP Addresses
```powershell
./Convert-CIDRInfo.ps1 -NetworkAddress '172.16.0.0/12' -Enumerate
```
