Name: Mary Precious Feutsop Ngouane

Level 0
I log into the game using the command:
ssh -p 2220 bandit0@bandit.labs.overthewire.org
I was promted to enter the password which was given as:  bandit0

Level 0 -> Level 1
List the files present in the home directory : ls
Open the readme file to see the content: cat readme
password:  ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
use ssh to log into the next level with the password found.

Level 1 -> Level 2
List the files present in the home directory : ls
The file name - doesn't work with cat. This confuses the command.
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
List all files including hidden ones: ls -a
Open the hidden file: cat ...Hiding-From-You
password: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

Level 4 -> 5