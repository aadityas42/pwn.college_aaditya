# Matching with []
The challenge requires us to use '[]' operators.

## My Solve
**Flag:**  'pwn.college{4IehDJCvt9HTgNfRY-BoOKsnSZs.QXzIDO0wSM0AzNzEzW}'

First we change our cwd to files, and then we execute the '/challenge/run file_[bash]' command, here, any one of the charecters: 'b','a','s','h' can be accpeted to complete the pattern.

```
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{4IehDJCvt9HTgNfRY-BoOKsnSZs.QXzIDO0wSM0AzNzEzW}
```

## What I learned
I learned that you can provide a subset of potential charecters within the '[]' brackets to match patterns in file globbing.

## References
Nil.
