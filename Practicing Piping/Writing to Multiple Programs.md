# Writing to Multiple Programs
The challenge requires you to pipe the output of one command to two others, combining concepts from previous two challenges.

## My Solve
**Flag:**  'pwn.college{k791EeVMyRZkS3vT7iFurFJ4hXl.QXwgDN1wSM0AzNzEzW}'

We execute the '/challenge/hack |tee >( /challenge/the) | /challenge/planet' command, which redirects the ouput of the '/challenge/hack' comand to the two others. For this, we use the 'tee' operator to intercept the output and copy it to the '/challenge/the' program as well, before letting it pass into the '/challenge/planet'program, which completes the requirement of the challenge.

```
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack |tee >( /challenge/the) | /challenge/planet
Congratulations, you have duplicated data into the input of two programs! Here 
is your flag:
pwn.college{k791EeVMyRZkS3vT7iFurFJ4hXl.QXwgDN1wSM0AzNzEzW}
```

## What I learned
I learned how to pipe outputs to two commands at once, this uses a combination of the knowledge obtained from the previous two challenges, which increases both the difficulty and potential power of using the commands together.
Using multiple operators like '|', '<','>' together can prove to be a very powerful tool and can help us represent the same command in multiple different ways, some being more readable than others.

## References
Nil.
