OverTheWire: Bandit - Level 3 to Level 4

Objective

Find the password for the next level. The password is stored in a hidden file located inside the inhere directory.

Commands Used

* ssh: Used to connect to the remote server as bandit3.
* ls: Used to list directory contents.
* cd: Used to navigate between directories.
* cat: Used to display the contents of a file.

Step-by-Step Solution

1. Connect to the Server

ssh bandit3@bandit.labs.overthewire.org -p 2220

Use the password obtained from Level 2 to log in as bandit3.

2. List the Directory Contents

ls

Output:

inhere

3. Navigate to the Directory

cd inhere

4. Display Hidden Files

By default, the ls command does not show hidden files. To reveal them, use the -a option:

ls -a

Output:

.  ..  ...Hiding-From-You

5. Read the Hidden File

cat ...Hiding-From-You

Output:

[next_level_password]

6. Save the Password

The password displayed in the hidden file is used to log in as bandit4.

Key Concepts Learned

* Understanding hidden files in Linux.
* Using the ls -a command to display hidden files and directories.
* Navigating the filesystem with cd.
* Reading file contents with cat.

Notes

This level introduces hidden files, a common feature in Unix-like operating systems. Files whose names begin with a dot (.) are hidden by default and often contain configuration data. Knowing how to locate and inspect hidden files is a fundamental Linux administration and cybersecurity skill.
