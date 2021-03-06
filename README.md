# ExtraUtils
A set of extra utilities made in Lua

This is a multi-call binary, like [Busybox](https://busybox.net/)

Therefore, the applet used will depend on the program name (a copy or link named moar will work like the moar applet)

Installation
---
Clone the repo, move the file to /usr/bin/ ,link every file with ``ln -s extrautils program`` and enjoy

Remember that the file can be minified, but be sure that the functions with names similar to the applets remain with that name

Currently contains:
---

**List**

Outputs the name of every program (excluding itself and extrautils) to standard output

**Moar**

A terminal pager similar to more with syntax highlighting for manual pages, also can read from files and from standard input

**CR**

Character Read, reads from a file or from standard input and outputs the ascii code (0-255) of every key

**FM**

File Manager, displays directories, links and files, with the option to create empty files, remove files and go to other folders

**LClock**

Lua Clock, add 'c' as a first argument for color, and 'p' to make it update and stay until killed, both can be combined

**Progr**

Outputs a progress bar with a percentage equal to the first argument

**Spinner**

Outputs a spinning bar next to a word equal to the first argument, this bar spins as much as the second argument indicates

**TED**

My Cli Text EDitor, also available as a single file [here](https://bowuigi.github.io/TED/) (documentation included)

**GAX**

GitHub Adress Expander, uses the first and second argument as Username and Repo respectively, and outputs the url needed to ``git clone``

**Coot**

Works like 'cut -d -f', except it only checks once instead of every line
First argument is the delimiter (can be only one character long but that is automatically autocorrected and the second argument is the field displayed, if there is no field then it will display 'invalid or null field'
