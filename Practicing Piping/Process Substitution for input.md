# Processing Substitution for Input
The challenge requires you to pipe the output of one command to another.

## My Solve
**Flag:**  'pwn.college{QxIe1wMjhvCbxPP8Zgu4PuTEzwW.0lNwMDOxwSM0AzNzEzW}'

First we execute the 'diff <( /challenge/print_decoys) <( /challenge/print_decoys_and_flag)' command to pipe the output of 'print_decoys' and 'print_decoys_and_flag' to the diff function as arguments so that we can get the difference between the two which is basically the flag since the decoys get destroyed in the 'diff' command. 

```
hacker@piping~process-substitution-for-input:~$ diff <( /challenge/print_decoys) <( /challenge/print_decoys_and_flag)
37a38
> pwn.college{QxIe1wMjhvCbxPP8Zgu4PuTEzwW.0lNwMDOxwSM0AzNzEzW}

```

## What I learned
I learned that the we can pipe outputs as arguments for other commands also. This is due to the philosophy of Linux that 'everything is a file'. This allows us to 'pass of' even commands as files to help pipe outputs directly into commands, by storing it intermediately in a file that is created by the shell.

## References
Nil.
