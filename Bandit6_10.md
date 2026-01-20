Bandit 6-7→

command used → find / (to list everything present on the directory (not recommended cuz takes too much time) 

find / -user bandit7 -group bandit6 -size 33c 2>/dev/null 

-user bandit7 -group bandit6 -size 33c was used cuz we were given 3 hints which were 

- owned by user bandit7
- owned by group bandit6
- 33 bytes in size

2>/dev/null is used to filter out/hide the errors

Password:-  m

Bandit 7-8→

command used → ls, grep “millionth” data.txt

grep command is used s**earch for specific text patterns** within files or data streams.

Password:- 

Bandit 8-9→

commands used→ sort data.txt | uniq -c

since there was a hint that the only line of text that occurs only once is the password, we used the uniq command. But in order to use this command we have to first sort the data.

sort data.txt is used to sort the data

uniq  is used to find the duplicate files and -c is used to count the number of times that data repeats.

Password:- 

Bandit 9-10→

commands used→ strings -n 10 data.txt

By default, `strings` outputs a lot of "garbage" (short sequences of random characters that happen to be printable). To get actual sentences or meaningful words, increase the minimum length using the `-n` flag.

Password:- 

Bandit 10-11→

commands used→ ls, cat data.txt, echo “example” | base64 -d

The base64 command in Linux is a simple utility for encoding and decoding data 
using the Base64 encoding scheme. It reads from standard input or a file
and writes to standard output. 

Password:- 
