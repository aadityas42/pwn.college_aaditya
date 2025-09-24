# Comparing Files
The challenge requires you to use the 'diff' command to check for changes in similar files.

## My Solve
**Flag:**  '> pwn.college{0iuRmW48LfrZGcfCRxLk9sCu8z_.01MwMDOxwSM0AzNzEzW}'

I used the 'diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt' command where diff is the command that checks the difference between the two files /challenge/decoys_only.txt and /challenge/decoys_and_real.txt as the first one has 100 fake flags and the second one has 100 fake flags along with 1 real fla. So the difference between these two flags gives the 1 real flag.

```
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
64a65
> pwn.college{0iuRmW48LfrZGcfCRxLk9sCu8z_.01MwMDOxwSM0AzNzEzW}
```

## What I learned
I learned that that diff operator is useful while trying to find differences in similar files rather than just trying to find the difference between them manually by observation.
Consider this example where:
'cat file1' yield this result:  Hello 
                                Hackers
'cat file2' yields this result: Hello
                                User
In such a scenario, the command 'diff file1 file2' will give the output:
2c2
< Hackers

> User

2c2 indicates that line 2 has changed.

Similarly, if file1 didnt have the second sentence 'Hackers', our output would be 1c2 instead of 2c2 which basically means that after line1 of file1, add line2 of file2, to get the change between the two files.

## References
Nil.
