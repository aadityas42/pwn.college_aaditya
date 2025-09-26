# Multiple Globs
The challenge requires us to use the concept of multiple globbing.

## My Solve
**Flag:**  'pwn.college{sRh_Se8UXudMp15qDfbO0GVOyUn.0lM3kjNxwSM0AzNzEzW}'

We first change our cwd to files, and then execute '/challenge/run *p*' which covers every file containing the letter 'p' which is all we need to meet the conditions of this challenge.

```
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{sRh_Se8UXudMp15qDfbO0GVOyUn.0lM3kjNxwSM0AzNzEzW}
```

## What I learned
I learned that we can provide multiple globs in a single argument, this can be done by providing a globbed word between two '*' operators. Such a glob covers all the files which contain the globbed word.

## References
Nil.
