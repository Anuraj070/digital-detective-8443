# Mission 5 - Numbers and data

## Task 5.1 - Convert numbers by hand

| Question | Your working and answer |
|---|---|
| Convert decimal 13 to binary. | $13 \div 2 = 6$ R1; $6 \div 2 = 3$ R0; $3 \div 2 = 1$ R1; $1 \div 2 = 0$ R1. Reading remainders bottom-to-top gives **1101**. |
| Convert decimal 25 to binary. | $25 \div 2 = 12$ R1; $12 \div 2 = 6$ R0; $6 \div 2 = 3$ R0; $3 \div 2 = 1$ R1; $1 \div 2 = 0$ R1. Reading remainders gives **11001**. |
| Convert binary 1010 to decimal. | $(1 \times 2^3) + (0 \times 2^2) + (1 \times 2^1) + (0 \times 2^0) = 8 + 0 + 2 + 0 =$ **10**. |
| Convert binary 1101 to decimal. | $(1 \times 2^3) + (1 \times 2^2) + (0 \times 2^1) + (1 \times 2^0) = 8 + 4 + 0 + 1 =$ **13**. |
| Convert hexadecimal A to decimal. | In base 16, digit A represents decimal value **10**. |
| Convert hexadecimal 1F to decimal. | $(1 \times 16^1) + (15 \times 16^0) = 16 + 15 =$ **31**. |
| Convert binary 1111 to hexadecimal. | Decimal value is $8 + 4 + 2 + 1 = 15$. In hexadecimal, 15 is represented as **F**. |

## Task 5.2 - Verify using Python

| Expression tested | Python output | Matches manual calculation? |
|---|---|---|
| `bin(13)` | `'0b1101'` | Yes |
| `bin(25)` | `'0b11001'` | Yes |
| `int("1010", 2)` | `10` | Yes |
| `int("1101", 2)` | `13` | Yes |
| `int("A", 16)` | `10` | Yes |
| `int("1F", 16)` | `31` | Yes |
| `hex(0b1111)` | `'0xf'` | Yes |

## Task 5.3 - Build a small number converter

I created and tested `number_converter.py`, which reads a decimal integer from the user and outputs its binary and hexadecimal equivalents.

| Test number | Binary output | Hexadecimal output |
|---|---|---|
| 10 | `0b1010` | `0xa` |
| 25 | `0b11001` | `0x19` |
| 42 | `0b101010` | `0x2a` |

- **Function explanation:**  
  - `bin()` takes an integer and returns its binary string prefixed with `0b`.  
  - `hex()` takes an integer and returns its hexadecimal string prefixed with `0x`.

## Task 5.4 - How is text stored?

- **ASCII decimal codes:**
  - Uppercase `A`: `65` (checked with `ord('A')`)
  - Lowercase `a`: `97` (checked with `ord('a')`)
- **Why encoding standards are needed:**  
  Computers only operate on electrical binary states (0s and 1s). An encoding standard maps human characters to numeric binary values so text can be reliably saved, transferred, and displayed across different systems.
- **Example of non-ASCII character:**  
  The Indian Rupee symbol (`₹`) or emojis like `😊` are not in basic ASCII (which only includes values 0–127) and require multi-byte UTF-8 encoding.

---

## 1. Task 

Convert values between decimal, binary, and hexadecimal, verify with Python, create an interactive conversion script, and explain text encoding.

## 2. Work completed

Calculated 7 manual number conversions with working, checked them using Python built-in conversion functions, wrote and tested `number_converter.py` with 3 test numbers, and documented character encoding principles.

## 3. Commands 

- `python3`: Used Python interactive shell to verify conversions.
- `bin()`: Built-in function to convert integer to binary string.
- `hex()`: Built-in function to convert integer to hexadecimal string.
- `int(value, base)`: Converted binary and hex strings to decimal integers.
- `ord()`: Checked character code points for text encoding.
- `touch number_converter.py`: Created script file.
- `python3 number_converter.py`: Ran and tested the number converter.

## 4. My understanding

Computers represent all data (numbers, text, media) as binary bits. Hexadecimal provides a human-friendly shorthand for binary (each hex digit represents 4 bits). Character encodings like ASCII and UTF-8 assign unique binary numbers to letters and symbols so software can consistently interpret text.

## 5. Difficulties faced

Remembering that Python's `bin()` and `hex()` output prefixes (`0b` and `0x`), which indicate the number base.

## 6. How I resolved them

Observed the prefixes in Python interactive testing and verified that the digits following the prefix match manual calculations.

## 7. Evidence 

- `mission-05-numbers-data/number_converter.py`
- `mission-05-numbers-data/README.md`

## 8. Commit details

Commit message: `Build number converter and practise data representation`

The completed Mission 5 work was committed and pushed to GitHub on the main branch.