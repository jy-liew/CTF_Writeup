# Python Wrangling

# Overview
Category: General Skills

Points: 10

Competition: picoCTF 2021

# Description
Python scripts are invoked kind of like programs in the Terminal... Can you run this Python script using this password to get the flag?

# Solution
This challenge provides 3 files:

Python script: `ende.py`

Password file: `pw.txt`

Flag file: `flag.txt.en`<br><br>
I opened the `ende.py` script using Sublime Text and it mentions how to decrypt a file:
>"Examples:\n" +\
>
>"To decrypt a file named 'pole.txt', do: " +\
>       
>"'$ python "+ sys.argv[0] +" -d pole.txt'\n"

In Linux terminal, decrypt `flag.txt.en` using `ende.py` by entering:

`python3 ende.py -d flag.txt.en`.

Next, enter the password inside `pw.txt`: 
`dbd1bea4dbd1bea4dbd1bea4dbd1bea4`

# Flag
picoCTF{4p0110_1n_7h3_h0us3_dbd1bea4}
