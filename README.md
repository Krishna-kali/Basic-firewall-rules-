# Basic-firewall-rules-
Configure and test basic firewall rules to allow or block traffic
1. Windows(Using Built -in Firewall)
open windows powershell and type cmd
# Allow inbound HTTP (Port 80)
New-NetFirewallRule -DisplayName "Allow HTTP" -Direction Inbound -Protocol TCP -LocalPort 80 -Action Allow

# Allow inbound HTTPS (Port 443)
New-NetFirewallRule -DisplayName "Allow HTTPS" -Direction Inbound -Protocol TCP -LocalPort 443 -Action Allow
![image alt](
