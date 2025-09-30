# Exporting Variables
The challenge needs you to export a variable.

## My Solve
**Flag:**  'pwn.college{oB4Ok3Xnyfrr53QmIpineAm6xLQ.QXyYTN0wSM0AzNzEzW}'

First, we use the 'export PWN=COLLEGE' command to export and assign the value 'COLLEGE' to the variable 'PWN'.
Then, we execute the command 'COLLEGE=PWN' to assign the value 'PWN' to the variable 'COLLEGE' without exporting it.
Finally, we execute '/challenge/run' to check our work and get our flag.

```
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great 
job! Here is your flag:
pwn.college{oB4Ok3Xnyfrr53QmIpineAm6xLQ.QXyYTN0wSM0AzNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```

## What I learned
I learned how to export a variable to a child-shell of the main shell using 'EXPORT' variable. 
This is because by default you can't access a variable in another child-shell because you may have sensitive or weird data in them.

## References
Nil.
