# `Bash Commands
- `bash` confirms existence of bash
- `exit` closes terminal session
- `pwd` prints current working directory
- `cd [directory-name]` changes current working directory
- `cd ..` changes current working directory to parent directory
- `cd ~` changes current working directory to home directory
- `mkdir [directory-name]` creates a new directory
- `ls` prints a list of files and subdirectories
- `rm [filename]` removes a file
- `rm -r [directory-name]` removes directory
- `cp [filename] [directory-name]` copies a file to a directory
- `cp -r [copy-directory-name] [paste-into-directory-name]` copies a directory to another directory
- `touch` creates a new file

# `Git` Commands
- `git config --global username "[username]"` sets username (one time)
- `git config --global email "[email@email.com]"` sets email (one time)
- `git clone [url]` copy files from github to local (one time per directory)
- `git status` gets staging status of files
- `git add [filename]` stage a file
- `git commit -m '[message]'` commit a file with message
- `git push` update files from local to github
- `git pull` update files from github to local
- `git log` get staging log
- `git checkout` undo any edit to the file, which reverts to last save
- `git reset HEAD [filename]` undo `git add`, which unstages the file but preserves any changes
- `git reset HEAD~`  undo `git commit` and `git add` but preserves any changes