# Linking Files
The challenge requires you to link a file to the flag file using symbolic linking.

## My Solve
**Flag:**  'pwn.college{wck3dySV-6-0dxX7WGDxqTGlur1.QX5ETN1wSM0AzNzEzW}'

First we execute the 'ln -s' command to link the flag and not-the-flag files, so we can fool the system into thinking it is telling us the contents of not-the-flag when we will actually get the contents of the flag file.
Then, I get the flag from the catflag file.

```
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{wck3dySV-6-0dxX7WGDxqTGlur1.QX5ETN1wSM0AzNzEzW}

```

## What I learned
I learned how to link two files using symbolic linking to obtain otherwise unobtainable data.

## References
Nil.
