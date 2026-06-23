# CompTIA--securityPlus-Practices
my notes, solutions, and practices scripts for the Security+ certification and OverTheWire challenges 
[5:18 p.m., 23/6/2026] Valkiria : # OverTheWire: Bandit - Level 0 a Level 1

## Objetivo
Encontrar la contraseña para el siguiente nivel, la cual está guardada en un archivo llamado readme en el directorio de inicio (home).

## Comandos utilizados
- ssh: Para conectarse al servidor remoto.
- ls: Para listar los archivos del directorio.
- cat: Para visualizar el contenido del archivo.

## Solución paso a paso

### 1. Conexión al servidor

bash
ssh bandit0@bandit.labs.overthewire.org -p 2220


Contraseña del nivel 0:

text
bandit0


### 2. Listar el contenido del directorio

bash
ls


Salida:

text
readme


### 3. Leer el contenido del archivo

bash
cat readme


Salida:

text
[contraseña_del_siguiente_nivel]


### 4. Guardar la contraseña

La contraseña mostrada en el archivo readme se utiliza pa…
[5:19 p.m., 23/6/2026] Valkiria : OverTheWire: Bandit - Level 0 to Level 1

Objective

Find the password for the next level, which is stored in a file called readme located in the home directory.

Commands Used

* ssh: Used to connect to the remote server.
* ls: Used to list the files in a directory.
* cat: Used to display the contents of a file.

Step-by-Step Solution

1. Connect to the Server
ssh bandit0@bandit.labs.overthewire.org -p 2220

level 0 password:
bandit0

2.- List the Directory Contents 
ls

Output:
readme

3.- Read the File Contents:
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
