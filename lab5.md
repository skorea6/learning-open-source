# Lab6 : Note on Git

### Changes vs Snapshots
- Storing data as changes to the base version vs Storing data as snapshots
- Git uses 'snapshots'

### Version Control
- Local
- Centralized
- Distributed

### Three Staes in Git
- Modified
- Staged
- Comitted

- Moddifed -> Stage : Stage fixes
- Staged -> Comitted : Commit
- Comitted -> Modified : Checkout the project

### Git config
- Git configurations are stored in 3 levels:
  1. System level: --system option. Affects all uses and repositories on the system (file: /etc/gitconfig)
  2. Global (user) level: --global option. Affects all repositories of a current user (file: ~/.config/git/config)
  3. Local level: --local option. Specific to the current repository (file: .git/gitconfig)
 
- Each level overrides values in the previous level: system -> global -> local
```sh
$ git config --list
$ git config --list --show-origin
$ git config --global user.name "Min Joon Choi"
```

### Initializing a Repository in an Existing Directory
```sh
$ git init
```

### Checking Repository Status
```sh
$ git status
```

### Adding a new file to be staged (tracked)
```sh
$ git add [file_name]
```
- git add . : add all files to be staged

### Unstaging a file
```sh
$ git rm –cached [file_name]
```

### Ignoring a file
- make .gitignore file
- *.a : ignore all .a files
- !lib.a : but do track lib.a, even though you're ignoring .a files above
- /TODO : only ignore the TODO file in the current directory
- build/ : ignore all files in any directory named build

### Commit
```sh
$ git commit -m “commit message”
$ git log
```

### Change branch name
```sh
$ git branch
$ git branch -m master main
```
