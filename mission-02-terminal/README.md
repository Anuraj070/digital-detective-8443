# Mission 2 - Terminal and file management

## Task 2.1 - Basic Terminal operations
| Command | What it does | What I observed |
|---|---|---|
| `pwd` | Shows the full path of the current folder. | It showed the Digital Detective project folder. |
| `ls` | Lists files and folders in the current location. | It showed the mission folders, evidence folder, and README file. |
| `ls -l` | Shows a detailed list of files and folders. | It showed permissions, owner, size, date, and names. |
| `cd ..` | Moves to the parent folder. | My current location changed from the project folder to its parent folder. |
| `mkdir` | Creates a new folder. | It created the `terminal-practice` folder. |
| `touch` | Creates an empty file. | It created `original.txt` inside the practice folder. |
| `cp` | Makes a copy of a file. | It made a copy of `original.txt`. |
| `mv` | Moves or renames a file. | It renamed the copied file to `backup.txt`. |
| `cat` | Displays the contents of a file. | It showed both lines saved in `original.txt`. |

## Task 2.2 - Safe file practice
I created `terminal-practice` inside my assignment repository. I created `original.txt`, added two lines, copied the file, and renamed the copy to `backup.txt`.

- Replacing contents means old text is removed and new text takes its place. Adding text puts new text after the existing text.
- Copying makes another file while keeping the original. Moving changes the file location or name.
- `pwd` shows the full location of the folder I am working in.
- `ls` is useful because it lets me check which files and folders are present.

## Task 2.3 - Flags and pipes
`ls` showed the normal list of files and folders. `ls -lah` showed more details, included hidden files such as `.git`, and displayed readable sizes.

The `|` symbol sends the output of one command to another command. In `ls -lah | head -n 5`, `ls -lah` creates the detailed list and `head -n 5` shows only the first five lines.

## Task 2.4 - Package managers
I checked Homebrew using `brew --version` and viewed its installed packages using `brew list`. I did not install or remove any software.

A package manager helps install, update, and remove software from the Terminal. Homebrew keeps track of installed packages, which makes software management more organised.

## 1. Task / objective

Practise Terminal commands, manage files safely, understand flags and pipes, and learn about package managers.

## 2. Work completed

I used basic Terminal commands, created a safe practice folder, created and managed text files, compared directory listings, used a pipe, and checked Homebrew.

## 3. Commands / tools used

`pwd`, `ls`, `ls -l`, `ls -lah`, `cd`, `mkdir`, `touch`, `echo`, `cat`, `cp`, `mv`, `head`, `brew --version`, and `brew list`.

## 4. My understanding

The Terminal can be used to work with files and folders through commands. Flags change the output of commands, and a pipe sends output from one command to another.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- `mission-02-terminal/README.md`
- `terminal-practice/original.txt`
- `terminal-practice/backup.txt`

## 8. Commit details
    Commit message: Complete Terminal and file management mission

The completed Mission 2 work was pushed to GitHub on the main branch.