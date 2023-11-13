# Nice netcat...

# Overview
Category: General Skills

Points: 15

Competition: picoCTF 2021

# Description
There is a nice program that you can talk to by using this command in a shell: $ nc mercury.picoctf.net 22902, but it doesn't speak English...

# Solution
The "nice program" in the description refers to Netcat or NC. It is a versatile networking utility that serves various purposes in networking and system administration.

`nc mercury.picoctf.net 22902`

This command provided in the description establishes a TCP connection to the server at mercury.picoctf.net on port 22902.

After entering the command, a long list of numbers appears. The numbers range from 1 to 9, so I assume they are in decimal form.
Using CyberChef to convert the numbers from ASCII decimals to text reveals the flag.

Link: `https://gchq.github.io/CyberChef/#recipe=From_Decimal('Space',false)&input=MTEyIA0KMTA1IA0KOTkgDQoxMTEgDQo2NyANCjg0IA0KNzAgDQoxMjMgDQoxMDMgDQo0OCANCjQ4IA0KMTAwIA0KOTUgDQoxMDcgDQo0OSANCjExNiANCjExNiANCjEyMSANCjMzIA0KOTUgDQoxMTAgDQo0OSANCjk5IA0KNTEgDQo5NSANCjEwNyANCjQ5IA0KMTE2IA0KMTE2IA0KMTIxIA0KMzMgDQo5NSANCjEwMCANCjUxIA0KMTAwIA0KMTAyIA0KMTAwIA0KNTQgDQoxMDAgDQoxMDIgDQoxMjUgDQoxMCA`

# Flag
picoCTF{g00d_k1tty!_n1c3_k1tty!_d3dfd6df}
