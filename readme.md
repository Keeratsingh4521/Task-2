# Task-2
Steps to access the encrypted file :-

1. Download the following files : 

    `keenable.enc` (this file contains the encrypted message)
    `special.key` (this file contains the key to decrypt the message)

After downloading both files, follow these steps to decrypt the file.

1. **Open the terminal.**

2. **Now, go to the folder where both downloaded files are. currently we are in the root folder. we can use this command to go to the desired folder where you downloaded both files.**

This is my current location in the terminal.

```
keerat@keerat:~$ 

```
Now, I want to go to `Downloads` folder where both of my files are located. Then we'll use this command.

```
cd Downloads
```

After executing this code, we'll be in the Downloads folder :

```
keerat@keerat:~/Downloads$ 
```

Now as we are in the desired location, we'll decrypt the file using this command.
Please copy paste this code in your command line.

```
openssl enc -aes-256-cbc -d -salt -in keenable.enc  -out simz.html -pass pass:noni
```
After this, run this command:
```
xdg-open simz.html
```
This will open the decrypted file in your browser.