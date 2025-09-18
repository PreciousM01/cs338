Name: Mary Precious Feutsop Ngouane

Level 0
I log into the game using the command:
ssh -p 2220 bandit0@bandit.labs.overthewire.org
I was prompted to enter the password which was given as:  bandit0

Level 0 -> Level 1
List the files present in the home directory : ls
Open the readme file to see the content: cat readme
password:  ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
use ssh to log into the next level with the password found.

Level 1 -> Level 2
List the files present in the home directory : ls
The file named '-' doesn't work with cat. This confuses the command.
Use a different format specifying it is a file in the current directory: ./- 
password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx

Level 2 -> Level 3
List the files present in the home directory : ls
open the file : cat "./--spaces in this filename--"
Note: cat and ./ alone were not working even when using the quotes. 
password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

Level 3 -> Level 4
List the files present in the home directory : ls
navigate to the inhere folder: cd inhere
List all files including hidden ones: ls -a. (-a lists all files)
Open the hidden file: cat ...Hiding-From-You
password: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

Level 4 -> 5
List the files present in the home directory : ls
navigate to the inhere folder: cd inhere
List all files including hidden ones: ls -a
Open all the files using the command:  cat ./-file07 (File -file07 is the correct one). Looking through all the files is tedious and time consuming.
password: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

Level 5 -> Level 6
List the files present in the home directory : ls
Navigate to the inhere folder: cd inhere
Navigate to maybeinhere07: cd maybehere07
List all the files and their properties: ls -a -l
ls gives a table of files with permissions, links, owner, group, size, date, name.
Open the file which has byte size (5th column) 1033: cat .file2
password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

Level 6 -> Level 7
search for a file with the given properties: find / -type f -user bandit7 -group bandit6 -size 33c (c specifies the size is in bytes, f is for regular readable files)
/var/lib/dpkg/info/bandit7.password
password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

Level 7 -> Level 8
Look at the words around "millionth": grep -C 1 "millionth" data.txt (more: -A: after, -B: before)
It looks at the lines before and after, including the line with "millionth"
password: dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

Level 8 -> 9
List the files present in the home directory : ls
Sort the textfile data.txt, form a set (uniq) of the texts while counting their frequency(-c),  and sort the text in increasing frequency using:
sort data.txt | uniq -c | sort -n
password: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM (string that occurs only once)


Level 9 -> Level 10
List the files present in the home directory : ls
Print the human readable strings using: strings data.txt
password: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey (string with a lot of ===)

Level 10 -> Level 11
List the files present in the home directory : ls
Print the content of data.txt:  cat data.txt
decode the base64 content of the text file: echo "output" | base64 -d
password: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

Level 11 -> 12
List the files present in the home directory : ls
Print the content of data.txt:  cat data.txt
decipher the output rot13 text using tr: echo "output" | tr 'A-za-z' 'N-ZA-Mn-za-m'
password: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4