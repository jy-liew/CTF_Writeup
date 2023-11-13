# Wave a flag

# Overview
Category: General Skills

Points: 10

Competition: picoCTF 2021

# Description
Can you invoke help flags for a tool or binary? This program has extraordinarily helpful information...

# Solution
This challenge provides one "program" file: `warm`.

In Linux terminal, just typing `warm` does not execute the file. After viewing the permissions with `ls -la`, `warm` did not have executable permissions for root.
So, I added the permission by typing `chmod +x warm`.

Enter `./warm -h` to execute the file and invoke help flags.

# Flag
picoCTF{b1scu1ts_4nd_gr4vy_18788aaa}
