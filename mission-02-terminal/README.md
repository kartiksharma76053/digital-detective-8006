# Mission 2 — Become comfortable with the Terminal

## 1. Task / objective
Practice basic Terminal commands to check the current directory, list files, create folders and text files, copy and rename files, understand command flags and pipes, and learn what package managers like Homebrew do.

## 2. Work completed
Completed Tasks 2.1 through 2.4 inside the repository and `terminal-practice/` folder:
- **Task 2.1:** Practiced basic Terminal navigation and file commands and recorded what each does.
- **Task 2.2:** Created `terminal-practice/practice/`, created `notes.txt` with two lines of text, made a backup copy, and renamed it to `final_backup.txt` (along with `renamed.txt`).
- **Task 2.3:** Compared `ls` with `ls -lah` and piped `ls -lah` into `head -n 5`.
- **Task 2.4:** Checked Homebrew version (`Homebrew 7.0.9`) and listed installed packages without installing or removing anything.

### Task 2.1 — Explore basic Terminal operations

| Operation / command name | What it does | What I observed |
| :--- | :--- | :--- |
| Current-directory display (`pwd`) | Prints the full path of the folder I am currently in. | Showed `/Users/[redacted]/Desktop/digital-detective-8006`. |
| Directory listing (`ls`) | Lists visible files and folders in the current folder. | Showed `README.md`, `evidence`, and all `mission-*` folders. |
| Detailed listing (`ls -l`) | Shows file permissions, owner, size in bytes, and modified date. | Showed each folder and file on its own line with `drwxr-xr-x` or `-rw-r--r--`. |
| Change directory (`cd`) | Moves to another folder, such as `cd ..` for the parent folder. | Running `cd ..` moved me up to `/Users/[redacted]/Desktop`. |
| Create directory (`mkdir`) | Creates a new empty folder. | Created `terminal-practice/practice` without any output. |
| Create empty file (`touch`) | Creates an empty file if it does not exist yet. | Created an empty text file inside the practice folder. |
| Copy file (`cp`) | Makes a duplicate of a file with a new name or location. | Created a copy of `notes.txt` while keeping the original untouched. |
| Move / rename file (`mv`) | Moves a file to a new path or renames it. | Renamed the copied file to `final_backup.txt`. |
| Display file contents (`cat`) | Prints the text inside a file in the Terminal. | Displayed both lines saved inside `notes.txt`. |

### Task 2.2 — Practise file changes safely
Inside `terminal-practice/practice/`, I created `notes.txt`, added `"I am learning Terminal commands."` using `>`, and appended `"This is my Digital Detective assignment."` using `>>`. Then I verified both lines with `cat notes.txt` and made `final_backup.txt`.

- **Replacing vs. adding text:** Replacing (`>`) overwrites the whole file and erases old content, while adding to the end (`>>`) keeps existing lines and appends new text after them.
- **Copying vs. moving a file:** Copying (`cp`) leaves the original file where it is and makes a second copy. Moving (`mv`) takes the original file and places it at the new name or folder, so only one file remains.
- **What `pwd` provides:** It tells me the exact full path from the root `/` down to my current working directory so I always know where I am.
- **Why `ls` is useful:** It lets me quickly see what files and folders exist in my current location before running commands on them.

### Task 2.3 — Understand flags and pipes
- **Flags (`ls` vs. `ls -lah`):** Plain `ls` only shows names of non-hidden files. Adding `-l` shows detailed permissions and dates, `-a` reveals hidden files starting with `.` (like `.git` and `.DS_Store`), and `-h` turns byte counts into readable sizes like `6.0K` or `512B`.
- **Pipes (`ls -lah | head -n 5`):** The pipe symbol `|` sends the text output from the command on the left directly as input to the command on the right. Here, `ls -lah` produces the full detailed file list, and `head -n 5` keeps only the first 5 lines.

### Task 2.4 — Understand package managers
Checked with `brew --version` (`Homebrew 7.0.9`) and `brew list`.
A package manager like Homebrew lets you install, update, and remove command-line tools and apps using simple commands instead of downloading installers from websites. It also handles dependencies automatically so everything needed by a tool gets installed cleanly.

## 3. Commands / tools used
- `pwd`, `ls`, `ls -l`, `ls -lah`, `cd`, `mkdir`, `touch`, `cp`, `mv`, `cat` — Basic navigation and file operations.
- `echo` with `>` and `>>` — Writing and appending lines to `notes.txt`.
- `head -n 5` with `|` — Limiting output to the first 5 lines.
- `brew --version`, `brew list` — Checking Homebrew version and installed packages.

## 4. My understanding
Working in the Terminal is fast once you know a few basic commands. Flags let you adjust how a command behaves, and pipes let you chain small commands together so the output of one becomes the input of the next.

## 5. Difficulties faced
No major difficulties. I just had to be careful to use `>>` instead of `>` for the second line so I did not overwrite the first line.

## 6. How I resolved them
Double-checked the file with `cat notes.txt` right after writing each line.

## 7. Evidence / files
- `mission-02-terminal/README.md`
- `terminal-practice/practice/notes.txt`
- `terminal-practice/practice/final_backup.txt`
- `terminal-practice/practice/renamed.txt`

## 8. Commit details
Committed with message `"Document Terminal operations, flags, pipes, and Homebrew"` (following `"Complete Terminal and file management mission"`) and pushed to `origin/main`.
