# Matching Paths with []
The challenge requires us to use '[]' operators with absolute paths.

## My Solve
**Flag:**  'pwn.college{8MIpY5_9GIpqaW5lcAnWxPkYULx.QX0IDO0wSM0AzNzEzW}'

We execute the '/challenge/run /challenge/run file_[bash]' command, here, as we need to specify the absolute path of the files rather than the relative one.

```
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{8MIpY5_9GIpqaW5lcAnWxPkYULx.QX0IDO0wSM0AzNzEzW}
```

## What I learned
I learned how to use the '[]' operator in the case where we use an absolute path for a file rather than it's relative path, which is an increased complexity compared to the previous one, as it merges two concepts together.

## References
Nil.
