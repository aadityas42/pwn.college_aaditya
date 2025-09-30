# Printing Exporting Variables
The challenge needs you to export a variable and read all of the exported variable using the 'env' command and find the flag amongst them.

## My Solve
**Flag:**  'pwn.college{MrJgOxyr01A7N0A4_Mp1DkUiUkq.QX4UTN0wSM0AzNzEzW}'

First, we use the 'export PWN=COLLEGE' command to export and assign the value 'COLLEGE' to the variable 'PWN'.
Then, we execute the command 'env' command to read out all of the exported variables. 
Then, we simply find the flag variable amongst all of the exported variables that get printed.

```
hacker@variables~printing-exported-variables:~$ export PWN=COLLEGE
hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
HOSTNAME=variables~printing-exported-variables
PWN=COLLEGE
PWD=/home/hacker
MANPATH=/run/dojo/share/man:
DOJO_AUTH_TOKEN=4beef36466ecf7b9d6f5f376743312dba2ecff68271e37485d7ed29b454221ef
HOME=/home/hacker
LANG=C.UTF-8
FLAG=pwn.college{MrJgOxyr01A7N0A4_Mp1DkUiUkq.QX4UTN0wSM0AzNzEzW}
TERMINFO=/run/dojo/share/terminfo
TERM=xterm-256color
SHLVL=2
LC_CTYPE=C.UTF-8
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DEBIAN_FRONTEND=noninteractive
_=/run/dojo/bin/env
```

## What I learned
I learned how to read out all of the exported variables using the 'env' command.

## References
Nil.
