# Listing Processes
The challenge requires you to use the ps commad to find which process has the flag stored in it.

## My Solve
**Flag:**  'pwn.college{o6BpduQ-wi9WuH6w9tQIY4CgBxx.QX4MDO0wSM0AzNzEzW}'

We just need to execute the 'ps aux' command which will list all processes. Since we are told that the process containing flag is stored in the '/challenge' directory but has been renamed, we can find it in the list displayed by the command and then run it to get the flag.

<img width="1833" height="282" alt="image" src="https://github.com/user-attachments/assets/034700a0-b333-44ff-872f-e8af78aa4fce" />

## What I learned
I learned how to use the 'ps' command also known as 'process snapshot' or 'process status' to get a list of all the processes running on our system although, just by itself, the command isn't very useful. So, we use it with arguments like 'aux' and '-ef' which help us get useful parameters.

There are two main types os syntaxes we can use with the ps command:
the first one is the standard syntax: In this, '-e' stands for every, which lists every process and '-f' for full format which includes arguments also. These two can be combined into a single parameter as '-ef'.
The second one is the 'BSD' syntax: In this, a stands for listing processes for all users, u stands for user-readable format, and x for lisitng programs that aren't running in a terminal. These can be combined into a single argument called as 'aux'.
The ouputs from both the syntax are comparable, though they do have slight differences.

Each process has a process ID or PID which is a numeric identifier for that particular process.

We also get to see the amount of cpu time dedicated to a particular process at any given time.
## References
Nil.
