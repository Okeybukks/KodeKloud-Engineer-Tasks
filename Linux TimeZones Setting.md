## TASK
During the daily standup, it was pointed out that the timezone across Nautilus Application Servers in Stratos Datacenter doesn't match with that of the local datacenter's timezone, which is America/Argentina/Mendoza.



Correct the mismatch.

## Solution
```sudo timedatectl set-timezone "America/Mendoza"```