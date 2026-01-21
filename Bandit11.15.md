**Bandit 11-12→**

**Command used→** ls, cat data.txt, echo “the text” | tr ‘a-zA-Z’ ‘n-za-mN-ZA-M’

Rot13 is used for simple text obfuscation or decoding by piping text through them, like `echo "Hello" | tr 'a-zA-Z' 'n-za-mN-ZA-M'` or using `sed` for more complex scripts, as ROT13 just shifts letters by 13 positions (A->N, N->A). (not a useful command)

Password:- 

**Bandit 12-13→**

**Command used →**

**1:-** `mkdir /tmp/foldername` (making a separate folder in tmp directory because we don't have write permissions in Home)
**2:-** `cd /tmp/foldername`

**3:-** `cp ~/data.txt .` (copying the file to our current location)

`xxd -r data.txt > data.bin` (reverse the hex dump to binary)
`file filename` (to check the file type)

**Condition 1:- if gzip →**`mv filename filename.gz` (renaming the file)
`gzip -d filename.gz`

**Condition 2:- if bzip2 →**`mv filename filename.bz2bzip2 -d filename.bz2`

**Condition 3:- if tar →**`mv filename filename.tartar -xf filename.tar`

*Keep checking the file type after each condition and stop once it says ASCII text.*

**Once you see ASCII text →**`cat filename`

Password:-

**Bandit 13-14→**

**Command Used→**

ssh -i filename bandit14@localhost -p 2220
-i filename (this is the identity flag. Basically it tells the ssh server that this is my key file use it”

Password:- private key required

**Bandit 14-15→**

**Command Used→**

Password:-
