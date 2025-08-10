# Basic-firewall-rules-
Configure and test basic firewall rules to allow or block traffic
1. Windows(Using Built -in Firewall)
open windows powershell and type cmd
# Allow inbound HTTP (Port 80)
New-NetFirewallRule -DisplayName "Allow HTTP" -Direction Inbound -Protocol TCP -LocalPort 80 -Action Allow

# Allow inbound HTTPS (Port 443)
New-NetFirewallRule -DisplayName "Allow HTTPS" -Direction Inbound -Protocol TCP -LocalPort 443 -Action Allow
![image alt](https://github.com/Krishna-kali/Basic-firewall-rules-/blob/f15f89b19003b57752a1a61ec661649b5f327e52/IMG_20250810_203624_993.png)
![image alt](https://github.com/Krishna-kali/Basic-firewall-rules-/blob/f0ab1acf7c96401a8e7f73c2c8cca6bccef2f1ec/IMG_20250810_203627_595.png)

2. Block a specific IP address
# Block inbound traffic from 192.168.1.50
New-NetFirewallRule -DisplayName "Block Malicious IP" -Direction Inbound -RemoteAddress 192.168.1.50 -Action Block
![image alt](https://github.com/Krishna-kali/Basic-firewall-rules-/blob/7866b873cb9e054111e48fb9a2105c9451a59662/IMG_20250810_203629_751.png)
