OverTheWire: Bandit - Level 2 to Level 3

Objective

Find the password for the next level. The password is stored in a file named spaces in this filename located in the home directory.

Commands Used

* ssh: Used to connect to the remote server as bandit2.
* ls: Used to list the files in the current directory.
* cat: Used to display the contents of a file.

Step-by-Step Solution

1. Connect to the Server

ssh bandit2@bandit.labs.overthewire.org -p 2220

Use the password obtained from Level 1 to log in as bandit2.

2. List the Directory Contents

ls

Output:

spaces in this filename

3. Read the File Contents

Because the filename contains spaces, the shell interprets each word as a separate argument. To access the file correctly, either escape the spaces with backslashes (\) or enclose the filename in quotation marks.

Using quotation marks:

cat "spaces in this filename"

Alternative method using escaped spaces:

cat spaces\ in\ this\ filename

Output:

[next_level_password]

4. Save the Password

The password displayed in the file is used to log in as bandit3.

Key Concepts Learned

* Handling filenames that contain spaces in Linux.
* Understanding how the shell parses command-line arguments.
* Using quotation marks to treat a filename as a single argument.
* Escaping special characters with backslashes (\).

Notes

This level demonstrates how the Linux shell interprets spaces as argument separators. Learning how to properly reference filenames containing spaces is an essential skill for working efficiently in Unix-like environments.
