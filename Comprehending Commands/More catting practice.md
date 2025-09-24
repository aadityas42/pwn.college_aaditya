# More catting practice
The challenge requires you to use the 'cat' command to display the contents of a file on the terminal window.

## My Solve
**Flag:**  'pwn.college{AY_IqPq0alpi4XW4nN_QkClQ9Xp.QXwITO0wSM0AzNzEzW}'

I used the 'cat /usr/include/rdma/flag' command to output the contents of the flag file. We are told that the flag is stored in the '/usr/include/rdma/flag directory' so I simply gave the given directory as the argument for the cat command to obtain the flag.

```
You cannot use the 'cd' command in this level, and must retrieve the flag by 
absolute path. Plus, I hid the flag in a different directory! You can find it 
in the file /usr/include/rdma/flag. Go cat it out **without** cding into that 
directory!
hacker@commands~more-catting-practice:~$  cat /usr/include/rdma/flag
pwn.college{AY_IqPq0alpi4XW4nN_QkClQ9Xp.QXwITO0wSM0AzNzEzW}
```

## What I learned
I got accustomed to using more complicated paths as the arguments for the cat command in cases where we can't use 'cd' to switch our cwd to the desired directory, the contents of which we want. 

## References
Nil.
