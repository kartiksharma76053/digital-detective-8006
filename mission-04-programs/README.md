# Mission 4 — How programs run

## 1. Task / objective
Create and run a simple one-line Python program (`hello.py`) from Terminal, and compare how compilers and interpreters translate and run code.

## 2. Work completed
- Created `mission-04-programs/hello.py` with `print("Hello from Python")`.
- Ran it from Terminal using `python3 mission-04-programs/hello.py` and confirmed `Hello from Python` appeared on screen.
- Completed the compiler vs. interpreter comparison table and short explanation.

### Task 4.2 — Compare compiler and interpreter

| Point | Compiler | Interpreter |
| :--- | :--- | :--- |
| When translation / execution happens | Translates the whole program before it runs. | Reads and runs the program line by line at runtime. |
| Typical output | Produces an executable file (like machine code). | Runs the program directly without making a separate executable file. |
| One example | C (using `gcc`) | Python (using `python3`) |
| One advantage | The compiled program usually runs very fast once built. | Easy to test and run code right away without a separate compile step. |

**Difference between a compiler and an interpreter:**
As shown in the table, a compiler translates the entire source code into machine code before the program starts, creating a separate executable file. Because all translation is done beforehand, compiled programs like C usually run faster. An interpreter, such as Python, reads and executes instructions directly at runtime without creating an executable file first. This makes Python very quick to write, test, and run while learning.

## 3. Commands / tools used
- `python3 mission-04-programs/hello.py` — Ran the Python script and printed `Hello from Python`.

## 4. My understanding
Computers cannot run human-readable Python or C code directly—it has to be translated or executed. Python uses an interpreter, so I can edit `hello.py` and run it right away with `python3` without compiling it first.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-04-programs/hello.py`
- `mission-04-programs/README.md`

## 8. Commit details
Committed with message `"Compare compilers and interpreters"` and pushed to `origin/main`.
