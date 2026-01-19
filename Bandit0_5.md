Bandit 0-1→

commands used → ls, cat

Passwords:- ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

Bandit 1-2→

commands used→ ls, cat ./- (./ is used to open dashed named files)

Password:-  263JGJPfgU6LtdEvgfWU1XP5yac29mFx

Bandit 2-3→

command used → ls, cat ./’—spaces in this filename—’

Reason → the file name was —spaces in the filename—

we cannot use cat —spaces in the filename— because the spaces are taken as a separate argument. so in order to avoid that we will use “ “ so first we will mention the current directory which can be written as ./ 

password:- MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

Bandit 3-4→

command used → ls, cd, ls -A (lists down all the files that are hidden excluding the , and .. entries which are showed when using ls -a)

password:- 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

Bandit 4-5→ 

command used → ls, cd, file ./*, cat ./-file07

if there are multiple files and identify what type of datas are inside it then we will use ./* command to identify the files. 

password:- 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

Bandit 5-6→

commands used→ file ./* → to look at every file in the current folder

find . -size 1033c → to find for directory which size was 1033 bits. cause there was a hint regarding the size of the file where the password was present. find command tool is used for searching files and directories based on various criteria, including name, size, type, modification time, and owner. 

password:- HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
