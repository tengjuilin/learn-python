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
