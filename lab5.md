# Lab5 : Note on Shell Commands

### I/O Redirection : Standard output
- ">" : redirect output using ">" after command to create and save the output in a file
```sh
$ ls -lh > file_list.txt
```
- ">>" : appends output to an existing file (if it already exitsts) or create and write to a new file if it doesn't exist.
```sh
$ ls -lh >> file_list.txt
```
- mix "<" and ">" together in a single line
- sort words.txt file first and then save in sorted_words.txt
```sh
$ sort < words.txt > sorted_words.txt
```

### Pipelines "|"
- Pipeline feeds output of previous command to input of next command
- command1 | command2 | command3
```sh
$ ls -lh | less
```

### Expansion
- echo text : print the text
```sh
$ echo print out the text
```
- echo * : print the all file names
```sh
$ echo *
```
- echo ~ : print the home directory
```sh
$ echo ~
```

### Backslash
- \ : to ignore line change in command("enter"), to enter a long command in multiple lines.
```sh
$ ls -l \
$  --reverse \
$  --human-readable
```

### Permissions
- Linux is a multi-user system.
- Files and directories have a permission assigned differently to owner / group / others.
```sh
$ ls -l /bin/bash
```
- -rwxrwxrwx : File Type(-: regular, d: directory), File Owner Permission(rwx), Group Owner Permission(rwx), Other User Permission(rwx)


### Changing Permissions
- chmod : changes permissions
```sh
$ chmod 600 some_file
```
- binary 600 = rw-------


### Superuser
- superuser : has all system administation authority.
- Some commands need superuser's privilleges.
- "sudo" : before the command if you are a superuser.
```sh
$ sudo some_command
$ sudo -i
```
- "sudo -i" : make superuser


### Text Editors
- In Linux, there is CLI-based or GUI-based text editors.
- vi, vim, emacs, nano, gedit, kwrite..


### Shell Script
- write a shell script
```sh
$ nano myscript.sh
```
- run a shell script
```sh
$ sh myscript.sh
```

### History
- "history" : to see previous command history.
- Or, save it to a text file.
```sh
$ history > history_command.txt
```
