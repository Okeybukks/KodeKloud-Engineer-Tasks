## Task
During the monthly compliance meeting, it was pointed out that several servers in the Stratos DC do not have a valid banner. The security team has provided serveral approved templates which should be applied to the servers to maintain compliance. These will be displayed to the user upon a successful login.



Update the message of the day on all application and db servers for Nautilus. Make use of the approved template located at /home/thor/nautilus_banner on jump host

## Solution 
1. Copy content of ```/home/thor/nautilus_banner```
2. ssh into the server
3. run ```sudo ln -s /etc/motd nautilus_banner```
4. Paste copied content into ```nautilus_banner```
