# Mission 5 — Numbers and data

## 1. Task / objective
Convert decimal, binary and hexadecimal values by hand, verify them with
Python, build a small number converter, and explain how text is stored.

## 2. Work completed

### Task 5.1 — Conversions by hand

| Question | Working and answer |
|---|---|
| Decimal 13 to binary | 13÷2=6 r1, 6÷2=3 r0, 3÷2=1 r1, 1÷2=0 r1. Reading remainders from the bottom up: 1101 |
| Decimal 25 to binary | 25÷2=12 r1, 12÷2=6 r0, 6÷2=3 r0, 3÷2=1 r1, 1÷2=0 r1. Reading upwards: 11001 |
| Binary 1010 to decimal | 1×8 + 0×4 + 1×2 + 0×1 = 10 |
| Binary 1101 to decimal | 1×8 + 1×4 + 0×2 + 1×1 = 13 |
| Hexadecimal A to decimal | A = 10 |
| Hexadecimal 1F to decimal | 1×16 + 15 = 31 |
| Binary 1111 to hexadecimal | 1111 = 8+4+2+1 = 15, and 15 is F, so F |

### Task 5.2 — Verification in Python

| Expression | Result | Matches my working? |
|---|---|---|
| `bin(13)` | `'0b1101'` | Yes |
| `bin(25)` | `'0b11001'` | Yes |
| `int("1010", 2)` | `10` | Yes |
| `int("1101", 2)` | `13` | Yes |
| `int("A", 16)` | `10` | Yes |
| `int("1F", 16)` | `31` | Yes |
| `hex(31)` | `'0x1f'` | Yes |
| `hex(int("1111", 2))` | `'0xf'` | Yes |

The `0b` and `0x` at the start only show which number system is used.

### Task 5.3 — number_converter.py

```python
number = int(input("Enter a positive decimal number: "))
print("Binary:", bin(number))
print("Hexadecimal:", hex(number))
```

| Test number | Binary output | Hexadecimal output |
|---|---|---|
| 10 | 0b1010 | 0xa |
| 25 | 0b11001 | 0x19 |
| 255 | 0b11111111 | 0xff |

- `input()` reads what the user types, as text.
- `int()` changes that text into a whole number.
- `bin()` gives the binary form of the number, starting with 0b.
- `hex()` gives the hexadecimal form, starting with 0x.

### Task 5.4 — How text is stored
- ASCII code of A is 65 and of a is 97.
- A computer only stores bits, so an encoding standard decides which number
  stands for which character. Without it, different programs could read the
  same bits as different text.
- A character outside basic ASCII: é (or ₹, or an emoji). UTF-8 can store it.

## 3. Commands / tools used
- python3: starts the Python interactive mode and runs my converter.
- bin(): converts a number to binary text.
- hex(): converts a number to hexadecimal text.
- int(): converts text to a number, and int(x, 2) or int(x, 16) reads
  binary or hexadecimal.
- input() and print(): read the user's number and show the results.
- ord(): gives the character code, used to check A and a.
- cd: moved into the mission folder to run the program.
- VS Code: wrote the program and this README.
- Git (status, add, commit, push): saved and uploaded the mission.

## 4. My understanding
Computers use bits, which are 0 or 1, and eight bits make a byte. Binary uses
base 2 and hexadecimal uses base 16, where A to F stand for 10 to 15.
Hexadecimal is a shorter way to write binary, because one hex digit equals
four bits. My converter takes a decimal number and uses Python's built-in
functions to show both forms. Text works the same way: each character has a
number code, and encodings like ASCII and UTF-8 define those codes.

## 5. Difficulties faced
No major difficulties. ]

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- mission-05-numbers-data/number_converter.py
- mission-05-numbers-data/README.md (manual working, Python checks, test
  results, encoding answers)

## 8. Commit details
- Commit message: Build number converter and practise data representation
- Pushed to GitHub: Yes 