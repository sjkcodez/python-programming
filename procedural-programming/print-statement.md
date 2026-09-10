# PRINT STATEMENT

### The print statement
__The print statement__ " print() " ; is a built-in function used to send human-readable text and data to the screen.

When you pass data into print("Hello, World!"), the computer automatically converts it into text, appends a invisible newline character (\n) so the next print statement drops to the next line.

   
## How Many Ways to Display Something on Screen in Python?

1. __The Standard print() Function__
The universal tool for all programmers. It is smart, handles complex text, and lets you print multiple data types at once.

Example:
```python
print("Hello, World!")
```

2. __The sys.stdout.write() Method__
print() is just a wrapper over Python's internal Standard Output (stdout) stream. By importing the sys module, you can write directly to the screen stream.

Unlike print(), it does not add a newline automatically
It only accepts pure strings (it will crash if you give it a number without converting it first)

Example
```python
import sys
sys.stdout.write("Hello, World!\n")
```

3. __The pprint Module__
Short for Pretty Print, this is a specialized built-in tool. If you try to print a massive dictionary or a long nested list with the standard print(), it will display as one, unreadable line. pprint breaks the data down into indented blocks automatically.

Example
```python
import pprint
data = {"user": "Alice", "hobbies": ["coding", "reading", "gaming"], "active": True}

pprint.pprint(data)
```

4. __The Interactive Expression Output__
If you are running Python inside an interactive terminal session (like the REPL prompt >>> or a Jupyter Notebook), you don't even need a function. Typing any raw variable name or expression and pressing Enter will automatically force Python to display its value on the screen

Example:
```python
>>> message = "Hello, World!"
>>> message
'Hello, World!'

```   

# The Evolution of Core Print Syntax

## 1. The Print Statement Era (Python 1.0 to 2.7)
In the early days of Python, print was a keyword statement rather than a function. No Parentheses were used, You did not use parentheses to wrap your message.
The entire Python 2 sequence officially reached its [End of Life (EOL)] on January 1, 2020. The PSF(Python Software Foundation) no longer writes patches, fixes bugs, or maintains Python 2 engines.


### Python 1 and 2 syntax
```python
print "Hello, World!"

```

## 2. The Print Function Era (Python 3.0 to Present)
Introduced in Python 3.0, print() became a standard built-in function. You must use parentheses to supply the text(Parentheses are Mandatory).
Launched in 2008, Python 3 introduced a massive update that broke backward compatibility. print() officially became a built-in function, making parentheses strictly 
Older Python 3 versions up to Python 3.9 (which hit EOL in October 2025) no longer work securely.mandatory.
The print function is fully operational and safely maintained on [Python 3.10, 3.11, 3.12, 3.13, and 3.14]

### Python 3 syntax
```python
print("Hello, World!")

```
