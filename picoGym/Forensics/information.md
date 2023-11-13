# information

# Overview
Category: Forensics

Points: 10

Competition: picoCTF 2021

# Description
Files can always be changed in a secret way. Can you find the flag? cat.jpg

# Solution
<p>This challenge provides one picture file: `cat.jpg`</p>
<img src=https://github.com/jy-liew/CTF_Writeup/assets/138641379/ad0e36f3-af18-45ab-9d2c-8707ba8d9d4d style="height: 300px">
<br><br>
<p>The picture has some artifacts so some information is hidden inside it. To find the hidden information, <code>exiftool</code> is used to read the metadata of the picture.</p>

<img height="500" alt="image" src="https://github.com/jy-liew/CTF_Writeup/assets/138641379/519deb4f-ea61-4b2d-a153-b5ccf969df98">
<br><br>
<p>
  There are 2 metadata that could be modified based on the characters used and length: "Current IPTC Digest" or "License".
  After using CyberChef to convert both from Base64, the flag is found in "Licence".<br><br>
  Link: <code>https://gchq.github.io/CyberChef/#recipe=From_Base64('A-Za-z0-9%2B/%3D',true,false)&input=Y0dsamIwTlVSbnQwYUdWZmJUTjBZV1JoZEdGZk1YTmZiVzlrYVdacFpXUjk</code>
</p>

# Flag
picoCTF{the_m3tadata_1s_modified}
