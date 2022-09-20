# Command-Line-Baics
## Reference
https://www.youtube.com/watch?v=uwAqEzhyjtw
https://gist.github.com/bradtraversy/cc180de0edee05075a6139e42d5f28ce

## Shortcuts
- `ctrl + L`  cleans the command line.
    - `clear` command do the same thing.
- `ctrl + R`  searches last related commands.

## General Commands
- `whoami` shows current user.
- `date` shows date.
- `touch file-{001..100}.txt`  creates 100 files with name pattern
- `ln -s locationxx shortcutxx`  creates a shortcut(symlink) to the location
- `tar -czvf dest.tar.gz src` create a zip
    - `tar -tzvf dest.tar.gz`  shows the contents of a zip
    - `tar -xzvf dest.tar.gz` unzips the zip into current directory
        - add `-C somefolder` to unzip to another directory
- `history` shows the past commands
    - `!number` reruns the past command

## Navigation
- `ls -a` shows hidden files.
- `ls -r`  shows reversed file list.
- `cd -`  navigates back to previous folder.
- `open xxx`  opens the folder or file or url.
    - on windows it's `start xxx`
- `cat - n xxx`  displays the content with line numbers.
- `nano xxx`  likes `vi`, but with more interactive instructions.
- `grep "abc" xxx` searches the term and returns the lines with the term.
    - term can be regex expression
        - ` "^private"` can search all lines start with private
        - `Local.*()` can search all lines with Localxxx()
- `find . -name "file-00*.txt"` can search for all files with the name pattern (in current and sub directories)
    - adding `-delete` deletes all files that have been found
