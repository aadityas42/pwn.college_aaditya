# Explicit Realtive Paths, from /
The challenge requires you to use . in your commands for relative paths to invoke a program.

## My Solve
**Flag:**  'pwn.college{kOBQfhktQN_p_-HqHpXCUggDgCN.QXwUTN0wSM0AzNzEzW}'

First we execute 'cd /' command to start from the / directory. Then I used the'./challenge/run' as the point of this challenge is to get comfortable with using . in our realative paths.

```
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{kOBQfhktQN_p_-HqHpXCUggDgCN.QXwUTN0wSM0AzNzEzW}

```

## What I learned
I learned that we can invoke programs while using .  in our directories as well, and got accustomed to using them in realtive paths. Also that the number of '/.' operators used doesn't matter and all paths with any number of the operator used can be considered as identitical.

## References
Nil.
