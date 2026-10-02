# OverTheWire-Writeups
This is a place i dedicated to writing my solutions to OverTheWire Bandit Challanges that i do to practice my Linux skills
## Level 0
The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.
- ssh bandit0@bandit.labs.overthewire.org -p 2220
## Level 1
The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.
- cat readme
- ssh bandit1@bandit.labs.overthewire.org -p 2220
## Level 2
The password for the next level is stored in a file called - located in the home directory
- cat ./-
## Level 3
The password for the next level is stored in a file called --spaces in this filename-- located in the home directory
- cat ./--spaces\ in\ this\ filename--
## Level 4
The password for the next level is stored in a hidden file in the inhere directory.
- cd inhere
- ls -a
- cat ...Hiding-From-You
## Level 5
The password for the next level is stored in the only human-readable file in the inhere directory. 
- Just checked each file and found the one i can read
## Level 6
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:
human-readable, 
1033 bytes in size, 
not executable.
- find . -type f -size 1033c ! -executable
## Level 7
The password for the next level is stored somewhere on the server and has all of the following properties:
owned by user bandit7, 
owned by group bandit6, 
33 bytes in size.
