# Command Line Notes/Learning

## Basic Navigation

### pwd

- [ ] (Where am I in the system.)

- [ ] (for unchecked checkbox)
- [x] (for checked checkbox)

### ls [path]

- [ ] (Perform a listing of the given path or your current directory.
Common options: -l, -h, -a)

### cd [path]

- [ ] (Change into the given path or into your home directory.)

### Path

- [ ] (A description of where a file or directory is on the filesystem.)

### Absolute Path

- [ ] (One beginning from the root of the file system (eg. /etc/sysconfig ).)

### Relative Path

- [ ] (One relative to where you currently are in the system (eg. Documents/music ).)

### ~ (tilde)

- [ ] (Used in paths as a reference to your home directory (eg. ~/Documents ).)

### . (dot)

- [ ] (Used in paths as a reference to your current directory (eg. ./bin ).)

### .. (dot dot)

- [ ] (Used in paths as a reference to your current directories parent directory (eg. ../bin ).)

### TAB completion

- [ ] (Start typing and press TAB. The system will auto complete the path. Press TAB twice and it will show you your alternatives.)

## More About Files

### file [path]

- [ ] Find out what type of item a file or directory is.

### Spaces in names

- [ ] Put whole path in quotes ( " ) or add a backslash ( \ ) in front of spaces.

### Hidden files and directories

- [ ] A name beginning with a . (dot) is considered hidden.

## Manual Pages

### man <command>

- [ ] View the manual page for a command.

### man -k <search term>

- [ ] Search for manual pages containing the search term.

### Press q to exit man pages

## File Manipulation

### mkdir <directory name>

- [ ] Create a directory.

### rmdir <directory name>

- [ ] Remove a directory (only if empty).

### touch <file name>

- [ ] Create a blank file.

### cp <source> <destination>

- [ ] Copy the source file to the destination.

### mv <source> <destination>

- [ ] Move the source file to the destination. May also be used to rename files or directories.

### rm <path>

- [ ] Remove a file or directory. Common options: -r -f

## Permissions

### r (read) w (write) x (execute)

### Owner or User, Group and Others

### ls -l [path]

- [ ] View the permissions of a file or all items in a directory.

### chmod <permissions> <path>

- [ ] Change permissions. Permissions can be either shorthand (e.g., 754) or longhand (e.g., g+x).

## Filters

### head

- [ ] Show the first n lines.

### tail

- [ ] Show the last n lines.

### sort

- [ ] Sort lines in a given way.

### wc

- [ ] How many words, characters and lines.

### grep

- [ ] Search for a given pattern.

- [ ] See more on our [Grep Cheat Sheet](https://www.gnu.org/software/grep/manual/grep.html#Regular-Expressions).

- [ ] More filters can be found [here](https://www.tecmint.com/15-basic-grep-command-examples-in-linux/).

## Useful Commands

### du -sh ./*

- [ ] Find the size of every directory in your current directory.

### df -h

- [ ] Display how much disk space is used and also free.

### basename -s .jpg -a *.jpg | xargs -n1 -i cp {}.jpg {}_original.jpg

- [ ] Make a copy of every jpg image file in the current directory and rename adding _original.

### find /home -mtime -1

- [ ] Find all files in the given directory (and subdirectories) which have been modified in the last 24 hours.

### shutdown -h now

- [ ] Shutdown the system. (Replace -h with -r for reboot.)

## Process Management

### CTRL + C

- [ ] Cancel the currently running process.

### kill <process id>

- [ ] Cancel the given process.
- [ ] Include the option -9 to kill a stubborn process.

### ps

- [ ] Obtain a listing of processes and their id's.
- [ ] Including the option aux will show all processes.

### CTRL + Z

- [ ] Pause the currently running process and put it in the background.

### jobs

- [ ] See a list of current processes in the background.

### fg <job number>

- [ ] Move the given process from the background to the foreground.

## Basic Usage

### vim or vi

- [ ] Run vim and open the given filename.

### :w

- [ ] Save file.

### :x or SHIFT ZZ

- [ ] Save and exit.

### :q

- [ ] Exit if no changes have been made.

### :q

- [ ] Exit and undo any changes made.

### :set nu

- [ ] Display line numbers.

## Deleting

### x

- [ ] Delete a single character.

### D

- [ ] Delete the rest of the line.

### dd

- [ ] Delete the entire current line.

### ndw

- [ ] Delete the next n words.

### ndd

- [ ] Delete the next n lines.

### :x,yd

- [ ] Delete from line x through to line y.

## Entering Insert mode

### i

- [ ] At the cursor.

### a

- [ ] After the cursor.

### I

- [ ] Before the current line.

### A

- [ ] After the current line.

### o

- [ ] Insert a new line after the current line.

### O

- [ ] Insert a new line before the current line.

### C

- [ ] Overwrite the whole current line.

### ESC

- [ ] Exit Insert mode.

## Movement

### h

- [ ] Move left one character.

### j

- [ ] Move down one character.

### k

- [ ] Move up one character.

### l

- [ ] Move right one character.

### w

- [ ] Move forward one word.

### b

- [ ] Move to the start of the word.

### e

- [ ] Move to the end of the word.

### (

- [ ] Move back one sentence.

### )

- [ ] Move forward one sentence.

### {

- [ ] Move back one paragraph.

### }

- [ ] Move forward one paragraph.

### ^

- [ ] Move to the beginning of the line.

### $

- [ ] Move to the end of the line.

### <n>G

- [ ] Move to the nth line.

### G

- [ ] Move to the last line.

### gg

- [ ] Move to the first line.

### %

- [ ] Move to the matching bracket.

## Search and Replace

### /pattern

- [ ] Search for pattern.

### n

- [ ] Find the next occurrence of pattern.

### :%s/pattern/replace/g

- [ ] Replace every occurrence of pattern with replace.

## Cut and Paste

### p

- [ ] Paste the clipboard contents.

### yy

- [ ] Yank (copy) a line.

### yw

- [ ] Yank a word.

### y$

- [ ] Yank to the end of the line.

## Additional Notes

- There are two types of paths **absolute** and **relative**. 
- **Absolute** paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )
- **Relative** paths specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.
- Everything is a file under linux.
- Linux is extentionless: Files can have any extension they like or none at all.
- Linux is case-sensitive.
- Remember you can easily look stuff up in the man pages. **Man (command)**, **man-k (search term)** Do a keyword search for all manual pages containing the given search term.
- Most commands have many useful command line options. Make sure you skim the man page for new commands so you are familiar with what they can do and what is available.
