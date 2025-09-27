# Multiple Options for Tab Completion
The challenge teaches us how to use tab completion when there are multiple available matches.

## My Solve
**Flag:**  'pwn.college{8xN7a9GyXUSD3Prs4GsDcCUawjB.0lN0EzNxwSM0AzNzEzW}'

First, we execute /challenge/files/pwn' and hit tab, which gives us a list of all matches with 'pwn' and from here, we check different files for the flag, the one named 'pwncollege-flag' is the one with the flag.

```
hacker@globbing~multiple-options-for-tab-completion:~$ /challenge/files/pwn
pwn                    pwn-the-planet         pwncollege-flamingo    pwncollege-hacking     
pwn-college            pwncollege-family      pwncollege-flyswatter
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/
hack-the-planet        pwn-college            pwncollege-family      pwncollege-flamingo    pwncollege-hacking     
pwn                    pwn-the-planet         pwncollege-flag        pwncollege-flyswatter  
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn
No flag in this file!
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-flag
pwn.college{8xN7a9GyXUSD3Prs4GsDcCUawjB.0lN0EzNxwSM0AzNzEzW}
```

## What I learned
I learned how to tab complete when multiple options are available and how in such a case should we choose which file to execute/check first.

## References
Nil.
