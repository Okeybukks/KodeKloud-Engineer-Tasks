## Task 
There is some data on Nautilus App Server 1 in Stratos DC. Data needs to be altered in several of the files. On Nautilus App Server 1, alter the /home/BSD.txt file as per details given below:



a. Delete all lines containing word software and save results in /home/BSD_DELETE.txt file. (Please be aware of case sensitivity)

b. Replace all occurrence of word and to them and save results in /home/BSD_REPLACE.txt file.

Note: Let's say you are asked to replace word to with from. In that case, make sure not to alter any words containing this string; for example upto, contributor etc.

## Solution

```sudo touch /home/BSD_REPLACE.txt```

```sudo touch /home/BSD_DELETE.txt```

```sudo chmod 666 /home/BSD_DELETE.txt```

```sudo chmod 666 /home/BSD_REPLACE.txt```

```grep -v following /home/BSD.txt > /home/BSD_DELETE.txt```

```sed 's/\bor\b/them/g' /home/BSD.txt > /home/BSD_REPLACE.txt```