<h1 align="center">Wargames</h1>

<h2>Game Info</h2>

Learning Resouce: <href>https://overthewire.org/wargames/</href>
The wargames offered by the OverTheWire community can help you to learn and practice security concepts in the form of fun-filled games.

<h2>Rules </h2>

Each Shell Game has it own SSH Port. 
Use the provided clues to find the password to the next SSH Port
NOTE: Whilst I've completed each task within this document, I've not provided the passwords, just the process I used to obtain the password. 

SSH Information
Host: bandit.labs.overthewire.org
Port: 2220

<h2>Bandit Tasks & Solutions </h2>

<h3>Level 1 Task</h3>
The password for the next level is stored in a file called <strong>readme</strong> located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

<h3>Level 1 Solution</h3>

Use SSH to log into Bandit0 session on Port 2220 
ssh bandit0@bandit.labs.overthewire.org -p 2220  
Enter the bandit0 password  
Use <strong>ls</strong> to list the directories  
<strong>Cat</strong> into the file  
Receive the password for Bandit1 log in
Log out of SSH

<h3>Level 2 Task</h3>
The password for the next level is stored in a file called <strong>-</strong> located in the home directory 

<h3>Level 2 Solution</h3>

Use SSH to log into Bandit1 session on Port 2220 
ssh bandit1@bandit.labs.overthewire.org -p 2220 
Use <strong>ls</strong> to list the directories 
The file is called <strong>-</strong> 
To open a file called <strong>-</strong> you must specify the full name of the file, which is <strong>./-</strong>
<strong>cat</strong> into the ./- file
Password received for Bandit3 
Log Out of SSH  

<h3>Level 3 Task</h3>
The password for the next level is stored in a file called <strong>spaces in this filename</strong> located in the home directory

<h3>Level 3 Solution</h3>

Use SSH to log into Bandit2 session on Port 2220 
ssh bandit2@bandit.labs.overthewire.org -p 2220 
Use <strong>ls</strong> to list the directories,  
The file is called <strong>spaces in file name</strong>
To access it you need to \ and space after each new word  
<strong>cat spaces\ in\ this\ filename</strong> 
File will open with the password, copy it  
Log out of SSH  

<h3>Level 4 Task</h3>
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command. 

<h3>Level 4 Solution</h3>

Log into the Bandit 3 session 
ssh bandit3@bandit.labs.overthewire.org -p 2220 
This has a hidden file in the directory, to find hidden files then us <strong>ls -a</strong> which will show all files including hidden ones.  
The file is called <strong>.hidden</strong>  
<strong>Cat</strong> into the .hidden file and the password is revealed.  
Copy password
Log out of SSH 
