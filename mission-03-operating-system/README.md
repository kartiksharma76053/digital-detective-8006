# Mission 3 — Understand the operating system

## 1. Task / objective
Explore the operating system, active user account, storage space, running processes, absolute vs. relative paths, file permissions, and the main responsibilities of an operating system.

## 2. Work completed
Completed Tasks 3.1 through 3.4 using Terminal commands and documented all observations safely without personal details.

### Task 3.1 — Explore your operating system

| Information explored | What it tells you | Your observation (privacy-safe) |
| :--- | :--- | :--- |
| Operating system / system details | Shows the OS name, version, kernel, and CPU architecture. | `macOS 26.7.3` (`Darwin 25.6.0 arm64`) |
| Current account identity | Shows which user account is currently logged in and running commands. | `[redacted]` (checked using `whoami`) |
| Available and used storage | Shows total disk size, used space, free space, and mount point. | `460Gi` total, `12Gi` used, `361Gi` available on `/` (4% used) |
| System activity snapshot | Shows running system and background processes at that moment. | Observed processes such as `launchd` (PID 1) and `logd` (PID 521) using `ps` |

### Task 3.2 — Understand processes
- **What is a process?** A process is a program that is currently loaded in memory and running on the computer.
- **What does the PID column represent?** PID stands for Process Identifier. It is a unique number the operating system gives to each running process so it can track and manage it.
- **Two examples of running processes:**
  1. `launchd` (PID 1) — the main system process on macOS that starts and manages background services.
  2. `Google Chrome` or `Code` (VS Code) — user applications running when I open a browser or editor.

### Task 3.3 — Understand paths and permissions
- **Absolute vs. relative path:** An **absolute path** starts from the root folder `/` and gives the full location of a file or folder no matter where I am. A **relative path** starts from my current working directory.
  - **Absolute path example:** `/Users/[redacted]/Desktop/digital-detective-8006/mission-03-operating-system`
  - **Relative path example:** `mission-03-operating-system` (when I am already inside `digital-detective-8006`)
- **File permissions check (`ls -l terminal-practice/practice/notes.txt`):**
  The permission string shown was `-rw-r--r--@`.
  The owner permission letters are `rw-` (the first three letters after `-`). This means the owner can **read (`r`)** and **write/edit (`w`)** the file, but **cannot execute (`-`)** it as a program.

| Permission | Meaning | Example |
| :--- | :--- | :--- |
| `r` — Read | Allows a file's contents to be read. | Opening a text file. |
| `w` — Write | Allows a file to be changed. | Editing a text file. |
| `x` — Execute | Allows a file to be run; on a directory, allows access/traversal. | Running a script. |

### Task 3.4 — Explain operating-system responsibilities

| OS responsibility | Your explanation | Example |
| :--- | :--- | :--- |
| Process management | Starts, schedules, and stops running programs so they share the CPU fairly. | Switching between Chrome and VS Code without crashing. |
| Memory management | Gives each running program RAM when it needs it and frees it when done. | Keeping open browser tabs and an editor in RAM at the same time. |
| Device management | Talks to hardware like keyboards, screens, and drives using drivers. | Sending text typed on the keyboard to the active window. |
| File management | Organizes data into files and folders on storage drives. | Saving `notes.txt` inside `terminal-practice/practice/`. |
| User interface / shell | Gives the user a way to interact with the OS, either visually or by typing commands. | macOS Finder (GUI) or Terminal with `zsh` (CLI). |
| Security and permissions | Controls who can log in and which files a user or app is allowed to read, edit, or run. | Checking `rw-` permissions before letting a user edit a file. |

## 3. Commands / tools used
- `sw_vers`, `uname -srm` — Checked macOS version and system architecture.
- `whoami` — Checked the current user account (redacted in notes).
- `df -h /` — Checked total, used, and available disk space.
- `ps -eo pid,comm | head -n 8` — Viewed running processes and their PIDs.
- `pwd`, `cd` — Tested moving between folders and comparing absolute vs. relative paths.
- `ls -l` — Checked owner permissions on `notes.txt`.

## 4. My understanding
The operating system sits between the hardware and the user. It keeps multiple programs running safely using PIDs, manages RAM and storage, and protects files with read/write/execute permissions so programs and users do not accidentally break things.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-03-operating-system/README.md`

## 8. Commit details
Committed with message `"Document operating system and file management"` and pushed to `origin/main`.
