# Named Pipes
The challenge requires you to create a FIFO and redirect an output to it.

## My Solve
**Flag:**  'pwn.college{4VI_TkVH0RyEu1IuL0_esIdNtkF.01MzMDOxwSM0AzNzEzW}'

We need to use two terminals for this challenge.
In the First, we execute 'mkfifo /tmp/flag_fifo' to make our desired FIFO. Then, we execute '/challenge/run > /tmp/flag_fifo' command to redirect the standard output to the FIFO.
Then, we open the second terminal and use the 'cat flag_fifo' command in it to get our flag, since FIFO operations are freezed until both the read and write sides of the pipe are executed.

```
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
hacker@piping~named-pipes:~$ cat flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at /tmp/flag_fifo! Here is your flag:
hacker@piping~named-pipes:~$ pwn.college{4VI_TkVH0RyEu1IuL0_esIdNtkF.01MzMDOxwSM0AzNzEzW}
```

## What I learned
I learned that we can create our own files to store the data we wish to pipe, such files are different from regular ones are called as FIFO.
FIFO have unique charecteristics: They don't take disk storage, erase their contents when read, block operations until both read and write sides of the 'pipe' are executed, and facilitate complex data flows in flexible ways.

## References
Nil.
