# Transformation

# Overview
Category: Reverse Engineering

Points: 20

Competition: picoCTF 2021

# Description
I wonder what this really is... enc 

`''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])`

# Solution
This challenge provides one file: `enc`

In Linux terminal, using `cat enc` to print the contents returns the following:

`灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸弲㘶㠴挲ぽ`

I can recognise some Chinese characters, so I assume this has something to do with Unicode.

Pasting the string above into CyberChef and using <b>Magic</b> tool with <b>Intensive mode</b> enabled, I was able to find the decoded flag.

# Flag
picoCTF{16_bits_inst34d_of_8_26684c20}
