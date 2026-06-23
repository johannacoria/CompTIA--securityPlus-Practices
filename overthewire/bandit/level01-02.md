OverTheWire: Bandit - Level 1 to Level 2

Objective

Find the password for the next level. The password is stored in a file named - (a single hyphen) located in the home directory.

Commands Used

* ssh: Used to connect to the remote server as bandit1.
* ls: Used to list the files in the current directory.
* cat: Used to display the contents of a file.

Step-by-Step Solution

1. Connect to the Server

ssh bandit1@bandit.labs.overthewire.org -p 2220

Use the password obtained from Level 0 to log in as bandit1.

2. List the Directory Contents

ls

Output:

-

3. Read the File Contents

Because - is interpreted as standard input/output by many Linux commands, it must be referenced explicitly using its relative path:

cat ./-

Output:

[next_level_password]

4. Save the Password

The password displayed in the file is used to log in as bandit2.

Key Concepts Learned

* Handling files with special characters in Linux.
* Understanding how commands interpret the hyphen (-) character.
* Using relative paths (./) to reference files unambiguously.
* Reinforcing basic file inspection techniques with the cat command.

Notes

This level introduces a common Linux challenge: working with filenames that have special meanings to shell commands. Understanding how to explicitly reference such files is an essential skill when navigating Unix-like systems 
