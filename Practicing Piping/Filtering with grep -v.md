# Filtering with grep -v
The challenge requires you to use the grep -v command to filter out decoys.

## My Solve
**Flag:**  'pwn.college{4xQBuwqowXnM1MqgNEYifHpfs7c.0FOxEzNxwSM0AzNzEzW}'

We execute the '/challenge/run | grep -v DECOY' command to filter out all strings with 'DECOY' in them, so we only get the real flag.
```
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{4xQBuwqowXnM1MqgNEYifHpfs7c.0FOxEzNxwSM0AzNzEzW}
```

## What I learned
I that grep can be used not only to match a string, but also to specifically mismatch/filter it out. Sometimes the only way to find what we want is remove what we don't. Grep -v proves to be useful in such cases.

## References
Nil.
