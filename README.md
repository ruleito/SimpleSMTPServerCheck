# SimpleSMTPServerCheck


Simple smtp server for check availible on 25 port Windows Server

requirements

open in firewall 25 port for any
powershell:

New-NetFirewallRule -DisplayName 'SMTP CHECK IN' -Profile 'Private' -Direction Inbound -Action Allow -Protocol TCP -LocalPort 25
New-NetFirewallRule -DisplayName 'SMTP CHECK OUT' -Profile 'Private' -Direction Inbound -Action Allow -Protocol TCP -LocalPort 25
