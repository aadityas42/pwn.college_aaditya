# Exclusionary Globbing
The challenge requires us to use '[]' operators with the '!' operator to exclude files.

## My Solve
**Flag:**  'pwn.college{cnMK4tLNGQl8sHyIQV7Dc6nzAYN.QX2IDO0wSM0AzNzEzW}'

First we change our cwd to files, and then execute '/challenge/run [!pwn]*' which ensures that files starting with 'p' or 'w' or 'n' are excluded.

```
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{cnMK4tLNGQl8sHyIQV7Dc6nzAYN.QX2IDO0wSM0AzNzEzW}
```

## What I learned
I learned how to use the '[!]' operator to exlcude files from a search or an execution, the '!' operator inverts the meaning of the '[]' operator.
## References
Nil.
