%title: intro_to_command_line (http://bit.ly/clgdi)
%author: milesmatthias.com
%date: 2014-09-21

# GDI upcoming events

#### Code &amp; Coffee
October 18th. 10a - 1p
Amante Coffee Baseline - Boulder

#### Intro to Programming with Ruby
October 25th. 9a-5:30p
Turing School - Denver

#### Intro to HTML/CSS
November 1 &amp; 2 1 - 5pm
SendGrid - Boulder

---

# about me

* senior developer at dojo4.com
* 17th & pearl st behind ted's
* stop by anytime! 

---

# history

* history
  * cpu
  * punch cards
  * terminal (unlimited access)
  * gui (mouse and graphics, sublime text)
* levels of abstraction
* why not use the gui all the time?

---

# shells

* a program that runs commands that you type in
* sh / bash / ksh,zsh,etc.
* microsoft windows
* prompt
  * user
  * host
  * location
* {cmd} {parameters}

---

# files

* files
* directories are just a type of file
  * 'directory' === 'folder'
* hidden files
* ls (-ahl)

---

# file hierarchy

* directories contain other directories and files
  * http://faculty.salina.k-state.edu/tim/unix_sg/_images/Unix_file_sys.png
* starts with /
* in the terminal, you're always inside a directory
* in the terminal, you type commands that manipulate files
* you can navigate to other directories to run commands on files
* you can also run commands on directories

---

# navigation

* pwd   - print working directory
* cd    - change directory
* mkdir - make directory
* rm    - remove ( -r / recursive )
* cp    - copy ( -R / recursive )
* mv    - move
* cat   - catenate
* echo  - display some text
  * echo > {file}
  * echo >> {file}

## notes:
* `.` === current directory
* `..` === directory one level up
* spaces and quotes
* asterisks (*)

---

# exercise 1

## file creation / navigation

* everyone good?

1. what directory are you currently in?
2. create a directory named `{your first initial}{your last name}` (ex: `mmatthias`)
3. change into your personal directory
4. create a file named `elephants` with the following text in it: `elephants are big`
5. make a directory named `animals`
6. move the file named `elephants` into the `animals` directory
7. rename `elephants` to `elephants.txt`
8. move your current directory to be in `animals`
9. print your current directory now
10. create a new file named `pandas.txt` with the following text in it: `pandas can be lots of colors`
11. copy `pandas.txt` to a file named `giraffes.txt`
12. print out the text in the `giraffes.txt` file
13. append the phrase `this file has incorrect content` to the `giraffes.txt` file
14. replace all of the text within the `giraffes.txt` file with the phrase `giraffes are really tall`
15. move your current directory one level up
16. copy the `animals` directory to a directory named `food`
17. print all of the text file contents in the `food` directory
18. remove the `food` directory
19. what directory are you in now?

---

# text editing, chaining, and scripting

* vim
  * read mode
  * arrow keys or hjkl
  * insert mode
  * escape
  * :w, :q, :wq
* chmod +x myscript.sh
* &&
* #!/bin/sh

---

# exercise 2 

## writing simple scripts

1. create a simple script named `cities.sh`
2. have the script print your name to the screen when executed
3. change the script to do the following when executed:
  1. create a file named `denver.txt` with the contents of `denver is cool`
  2. create a file named `boulder.txt` with the contents of `boulder is fun`
  3. make a directory named `colorado cities`
  4. move `denver.txt` and `boulder.txt` into the `colorado cities` folder
  5. print the contents of the text files within the `colorado cities` folder
  6. remove the `colorado  cities` folder
4. print text to the screen after each command in the script to show the script's progress (ex: 'just created denver.txt')
5. create a one-line command that does the same thing that this script does

---

# some tricks

* history
* !
* ctrl-r
* alias
* prompt (PS1)
* .bashrc
* source or . ./.bashrc

---

# screen

* screen -list
* screen -S [name]
* ctrl-a
  * c
  * d
  * exit
  * A
  * "
* screen -d -r [name]

---

# exercise 3

* alias some things
* customize your bash prompt
* run previous commands
* screen

---

# advanced bash / more unix-y

## file permissions

* chmod
* users
* chown
* groups
* chgrp

## user permissions

* /etc/passwd
* /etc/group
* sudo / root

---

# topics to research / experiment

* git
* tabs (both in terminal and in vim)
* links (symbolic vs hard)
* homebrew (mac only)
* awk, sed, grep


