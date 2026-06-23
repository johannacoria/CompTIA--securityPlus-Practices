OverTheWire: Bandit - Level 0 to Level 1

Objective

Find the password for the next level, which is stored in a file called readme located in the home directory.

Commands Used

* ssh: Used to connect to the remote server.
* ls: Used to list the files in a directory.
* cat: Used to display the contents of a file.

Step-by-Step Solution

1. Connect to the Server

ssh bandit0@bandit.labs.overthewire.org -p 2220

Level 0 password:

bandit0

2. List the Directory Contents

ls

Output:

readme

3. Read the File Contents

cat readme

Output:

[next_level_password]

4. Save the Password

The password displayed in the readme file is used to log in as bandit1.

Key Concepts Learned

* Basic SSH usage for accessing remote systems.
* Basic Linux navigation.
* Using the ls command to identify files.
* Using the cat command to read the contents of text files.

Personal Notes

This level serves as an introduction to the Bandit platform and basic interaction with a remote Linux system through the terminal.
