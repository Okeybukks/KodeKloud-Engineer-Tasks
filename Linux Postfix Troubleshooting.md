## Task
Some users of the monitoring app have reported issues with xFusionCorp Industries mail server. They have a mail server in Stork DC where they are using postfix mail transfer agent. Postfix service seems to fail. Try to identify the root cause and fix it.

## Solution
Check postfix status ```sudo systemctl status postfix -l```

Edit postfix configuration file
```sudo vi /etc/postfix/main.cf```

Comment ```#net_interfaces = localhost```

Restart postfix
```sudo systemctl restart postfix```