# why | Forensics | Hamza Haroon

Hint: I don't know why.

# Solution:

Given is a file named why.rar which is password protected. The password is pretty simple and hidden in plain sight. Yes, you guessed it right, “why”. 

![Untitled](why%20Forensics%20Hamza%20Haroon%2073ddecff1021420da4b0e5ff13703234/Untitled.png)

We get another zip file that is not password protected. Thank God!

We have two files in the folder.

![Untitled](why%20Forensics%20Hamza%20Haroon%2073ddecff1021420da4b0e5ff13703234/Untitled%201.png)

The audio is some total gibberish. while the file flag.txt is a .exe which is locked. 

Audacity or Sonic Visualizer is our best friend. We open the audio.

![Untitled](why%20Forensics%20Hamza%20Haroon%2073ddecff1021420da4b0e5ff13703234/Untitled%202.png)

The first thing to always check for in an audio file during any CTF is to check its spectrogram for any information. Let's see:

![Untitled](why%20Forensics%20Hamza%20Haroon%2073ddecff1021420da4b0e5ff13703234/Untitled%203.png)

![Untitled](why%20Forensics%20Hamza%20Haroon%2073ddecff1021420da4b0e5ff13703234/Untitled%204.png)

and VOILAAAAA!! We have a string that seems like Base64 encoded. Let's fire up Cyberchef and decrypt it.

![Untitled](why%20Forensics%20Hamza%20Haroon%2073ddecff1021420da4b0e5ff13703234/Untitled%205.png)

Seems like the question is giving us a tough time by telling us that we are on a dead end and the string is a password, not a flag. But wait, we have another file given to us that is password protected. This might be its password. Let's check:

![Untitled](why%20Forensics%20Hamza%20Haroon%2073ddecff1021420da4b0e5ff13703234/Untitled%206.png)

iamapasswordnotaflag is the password to the encrypted file. Now we have a file named flag.txt. Open it and you will find your flag.

`AOF{aud10_f0ren$1c$_1$_fun}`

Hope you enjoyed it.