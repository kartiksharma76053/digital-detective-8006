# Mission 5 — Numbers and data

## 1. Task / objective
Practice converting numbers by hand between decimal, binary, and hexadecimal, verify the answers in Python, build `number_converter.py`, and explain how computers store text using character encoding.

## 2. Work completed
Completed Tasks 5.1 through 5.4 and wrote `number_converter.py`.

### Task 5.1 — Convert numbers by hand

| Question | Your working and answer |
| :--- | :--- |
| Convert decimal 13 to binary. | 13 ÷ 2 = 6 rem 1; 6 ÷ 2 = 3 rem 0; 3 ÷ 2 = 1 rem 1; 1 ÷ 2 = 0 rem 1. Reading bottom to top: **1101** |
| Convert decimal 25 to binary. | 25 ÷ 2 = 12 rem 1; 12 ÷ 2 = 6 rem 0; 6 ÷ 2 = 3 rem 0; 3 ÷ 2 = 1 rem 1; 1 ÷ 2 = 0 rem 1. Reading bottom to top: **11001** |
| Convert binary 1010 to decimal. | (1 × 8) + (0 × 4) + (1 × 2) + (0 × 1) = 8 + 0 + 2 + 0 = **10** |
| Convert binary 1101 to decimal. | (1 × 8) + (1 × 4) + (0 × 2) + (1 × 1) = 8 + 4 + 0 + 1 = **13** |
| Convert hexadecimal A to decimal. | In hex, A = 10, so 10 × 16⁰ = **10** |
| Convert hexadecimal 1F to decimal. | (1 × 16) + (15 × 1) = 16 + 15 = **31** |
| Convert binary 1111 to hexadecimal. | 1111₂ = (1 × 8) + (1 × 4) + (1 × 2) + (1 × 1) = 15 in decimal = **F** in hexadecimal |

### Task 5.2 — Verify using Python
Tested the conversions in Python 3:

| Expression tested | Python output | Matches manual calculation? |
| :--- | :--- | :--- |
| `bin(13)` | `'0b1101'` | Yes (`1101`) |
| `bin(25)` | `'0b11001'` | Yes (`11001`) |
| `int('1010', 2)` | `10` | Yes (`10`) |
| `int('1101', 2)` | `13` | Yes (`13`) |
| `int('A', 16)` | `10` | Yes (`10`) |
| `int('1F', 16)` | `31` | Yes (`31`) |
| `hex(int('1111', 2))` | `'0xf'` | Yes (`F`) |

### Task 5.3 — Build a small number converter
Created `mission-05-numbers-data/number_converter.py` using `input()`, `int()`, `bin()`, and `hex()`.

- `bin(number)` converts an integer into its binary string starting with `0b`.
- `hex(number)` converts an integer into its hexadecimal string starting with `0x`.

**Test runs:**

| Test number | Binary output | Hexadecimal output |
| :--- | :--- | :--- |
| 13 | `0b1101` | `0xd` |
| 25 | `0b11001` | `0x19` |
| 255 | `0b11111111` | `0xff` |

### Task 5.4 — How is text stored?
- **ASCII decimal codes:** Uppercase `A` is `65` and lowercase `a` is `97`.
- **Why computers need an encoding standard:** Computers only store numbers (binary 0s and 1s), so an encoding standard gives every letter, digit, and symbol a fixed number so different computers read and display the same text.
- **Example of a character not in basic ASCII:** The Indian Rupee symbol `₹` (or an emoji like `😊`), which requires UTF-8 / Unicode.

## 3. Commands / tools used
- `python3` — Tested conversion expressions and ran `number_converter.py`.
- Python functions: `input()`, `int()`, `bin()`, `hex()`, `print()`.

## 4. My understanding
Everything inside a computer—numbers and text alike—is stored as bits (0 and 1). Binary and hexadecimal are just different ways of writing those values, and character encodings like ASCII and UTF-8 map characters to numbers so text can be saved and shared.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-05-numbers-data/number_converter.py`
- `mission-05-numbers-data/README.md`

## 8. Commit details
Committed with message `"Build number converter and practise data representation"` and pushed to `origin/main`.
