# Lab4 : Note on Shell Commands

### pwd
- shows the current path in hierachical directory

### cd, ls
- cd : change directory
- ls : list files and directories
- arguments :
  - [directory name]
  - / root
  - . current directory
  - .. uuper-level directory
  - /[directory name]: absolute path
  - ./[directory name]: relative path
  - ./[directory name]: relative path
- options:
  - -l : show detailed information (long format)
  - -lh : same as above, but size in units

### clear
- clear the shell

### cp
- copy files and directories
- cp file1 file2 : Copies the contents of file1 into file2.
- cp -i file1 file2 : "-i" (if file2 exists, the user is pormpted before it is overwritten with the contents of file1)
- cp file1 dir1 : Copy the contents of file1 inside of directory dir1.
- cp -R dir1 dir2 : Copy the contents of the directory dir1. If directory dir2 does not exist, it is created. Otherwise it creates a directory named dir1 within directory dir2.

### mv
- move files and directories or rename them
- mv file1 file2 : If file2 does not exist, then file1 is renamed file2. If file2 exists, its contents are silently replaced with the contents of file1.
- mv -i file1 dir1 : "-i" (if file2 exists, the user is pormpted before it is overwritten with the contents of file1)
- mv file1 file2 dir1 : The files file1 and file2 are moved to directory dir1. If dir1 does not exist, mv will exit with an error.
- mv dir1 dir2 : If dir2 does not exist, then dir1 is renamed dir2.

### rm
- delete files and directories ***permantely*** and ***irreversevely***
- rm file1 file2 : Delete file1 and file2

### mkdir
- make a new directory

### help
- help cd : the manumal of "cd" command

### man
- man cp : the manumal of "cp" command

### exit
- exiting the terminal
  
