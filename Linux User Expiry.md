## Task
A developer siva has been assigned Nautilus project temporarily as a backup resource. As a temporary resource for this project, we need a temporary user for siva. It’s a good idea to create a user with a set expiration date so that the user won't be able to access servers beyond that point.



Therefore, create a user named siva on the App Server 1. Set expiry date to 2021-02-17 in Stratos Datacenter. Make sure the user is created as per standard and is in lowercase.


## Solution
```sudo useradd -m -e 2021-02-17 -s /bin/bash siva```