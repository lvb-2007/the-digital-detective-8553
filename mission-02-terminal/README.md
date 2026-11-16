# Mission 2 BECOME COMFORTABLE WITHT HE TERMINAL

 
Commands / tools used: pwd, ls, ls -l, ls -lah, cd, mkdir, touch, cp, mv, cat, echo, >, >>, |, head, brew.

Difficulties: No major difficulties




 Work completed:
# task 2.1 EXPLORE BASIC TERMINAL OPERATIONS

| Operation | Command | What it does | What I observed |
|---|---|---|---|
| Current-directory display | `pwd` | Shows the full path of the folder I am in | It printed a path ending in my project folder, `/Users/[redacted]/.../the-digital-detective-8553` |
| Directory listing | `ls` | Lists the files and folders in the current location | It showed `README.md`, `evidence` and all the `mission-` folders |
| Detailed listing | `ls -l` | Lists the same items with permissions, owner, size and date | Each item was on its own line with permission letters like `-rw-r--r--`, the owner (`[redacted]`), size and modified date |
| Change directory | `cd ..` | Moves up to the parent folder | After `pwd`, the path was one folder shorter, so I was now outside my project folder |
| Create directory | `mkdir terminal-practice` | Makes a new folder | No message appeared, but `ls` then showed a new `terminal-practice` folder |
| Create empty file | `touch terminal-practice/notes.txt` | Makes an empty file | No message appeared, and `ls terminal-practice` showed `notes.txt` |
| Copy file | `cp terminal-practice/notes.txt terminal-practice/notes-copy.txt` | Duplicates a file under a new name, keeping the original | Both `notes.txt` and `notes-copy.txt` were in the folder |
| Move / rename file | `mv terminal-practice/notes-copy.txt terminal-practice/notes-renamed.txt` | Renames a file, or moves it to another place | `notes-copy.txt` disappeared and `notes-renamed.txt` appeared in its place |
| Display file contents | `cat terminal-practice/notes.txt` | Prints a file's contents in the terminal | Nothing was printed, because the file is empty |

### Task 2.2 — File changes in terminal-practice
Output of `cat practice.txt`:
This is the first line
This is the second line


1. Replacing vs adding to the end
Replacing (>) removes the old contents and writes the new text in their place. 
Adding (>>) keeps what’s already in the file and puts the new text after it. 
In my practice file, >> is why the first line was still there after I added the second.

2. Copying vs moving
Copying (cp) makes a second file, so the original stays where it is.
 Moving (mv) takes the file from one place to another, so only one copy exists afterwards. 
 Renaming is just moving a file to a new name in the same folder.

3. What the current-directory display (pwd) tells me
It prints the full path of the folder I’m working in, from the top of the file system down to my folder. 
It tells me where I am, so I know where new files will be created and what a relative path is measured from.

4. Why a directory listing (ls) is useful
It shows what files and folders are in the current location, so I can check that a command worked (for example, that a copy or rename really happened) and find the exact file name before using it.

# task 2.3 
 for ls -l 
-rw-r--r--@ 1 [redacted]  staff    0 Nov 16 13:36 README.md

for ls -lah
-rw-r--r--@  1 vidushibhatt  staff     0B Nov 16 13:36 README.md

for ls -l | head
-rw-r--r--@ 1 vidushibhatt  staff    0 Nov 16 13:36 README.md

# task 2.4 
brew -- version 
Homebrew 7.0.14

Why Package managers are useful ?

A package manager like homebrew lets me install software with a single command instead of searching for a website and downloading an installer by hand. It also makes updating and removing software easy and clean , because it keeps track of what it installed and where. On top of that , it automatically installs the other software a package depends on , so I don't have to find those extra pieces myself.
