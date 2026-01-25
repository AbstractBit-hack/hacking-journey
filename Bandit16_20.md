## Bandit 16-17→

**Command Used→**

`nmap -sV -n -p 31000-32000 localhost`

Next, connect to the identified port:

`openssl s_client -quiet -connect localhost:<port>`

Then, to save the RSA Private Key on your local computer:

`nano sshkey17.private`

(Paste the RSA Private Key here)

Set the appropriate permissions:

`chmod 600 sshkey17.private`

Finally, SSH into Bandit 17 using the private key:

`ssh -i sshkey17.private bandit17@bandit.labs.overthewire.org -p 2220`
