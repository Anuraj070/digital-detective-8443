# Mission 4 - How programs run

## Task 4.1 - Create and run a Python program

I created `hello.py` in the `mission-04-programs` directory with the following content:
```python
print("Hello from Python")
```

Running `python3 hello.py` in Terminal displayed:
```text
Hello from Python
```

## Task 4.2 - Compare compiler and interpreter

| Point | Compiler | Interpreter |
|---|---|---|
| When translation / execution happens | Translates the whole program into machine code all at once before running. | Translates and executes the code line-by-line at runtime. |
| Typical output | Standalone executable binary file (e.g., machine code file). | Directly executes in memory without producing a standalone executable file. |
| One example | C / C++ / Rust | Python / JavaScript |
| One advantage | Faster program execution speed because code is already compiled to machine instructions. | Easier testing and rapid prototyping without waiting for a build step. |

### Summary explanation
A compiler takes the entire source code and converts it into machine code before the program is executed, producing a standalone binary that runs very quickly. An interpreter reads and executes source code line-by-line dynamically at runtime. While compiled programs run faster, interpreted languages like Python make debugging and experimenting much quicker since changes can be run immediately.

---

## 1. Task / objective

Run a simple Python program and compare how compilers and interpreters translate and execute code.

## 2. Work completed

Created and ran `hello.py` using Python 3, observed the output in Terminal, and completed a comparison between compilers and interpreters.

## 3. Commands / tools used

- `touch hello.py`: Created the Python script file.
- `python3 hello.py`: Executed the Python program using the Python 3 interpreter.
- Text editor: Wrote the print statement inside `hello.py`.

## 4. My understanding

Compilers translate code completely into machine code before running, which makes execution fast. Interpreters execute code line-by-line at runtime, which simplifies testing and development. Python uses an interpreter to execute instructions directly.

## 5. Difficulties faced

Accidentally typed `print("Hello from Python")` directly into the zsh Terminal prompt instead of running it through Python or saving it into the file, which caused a shell error (`zsh: unknown file attribute: H`).

## 6. How I resolved them

Saved the Python print statement into `hello.py` and executed it properly using the command `python3 hello.py`.

## 7. Evidence / files

- `mission-04-programs/hello.py`
- `mission-04-programs/README.md`

## 8. Commit details

Commit message: `Compare compilers and interpreters`

The completed Mission 4 work was committed and pushed to GitHub on the main branch.