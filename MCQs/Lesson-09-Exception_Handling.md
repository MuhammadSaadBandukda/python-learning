# Lesson 09 - Exception Handling - MCQs

### 1. What exception is raised when the wrong data type is passed to a function?
A. `ValueError`  
B. `TypeError`  
C. `AttributeError`  
D. `SyntaxError`  
<details>
<summary>Answer</summary>
B. `TypeError` — Raised when an operation or function is applied to an object of inappropriate type.
</details>

---

### 2. What happens if `int('abc')` is executed?
A. `TypeError`  
B. `ValueError`  
C. `SyntaxError`  
D. `NameError`  
<details>
<summary>Answer</summary>
B. `ValueError` — Raised when a function receives an argument of correct type but inappropriate value.
</details>

---

### 3. Which exception would this code raise? `import non_existent_module`
A. `ModuleNotFoundError`  
B. `ImportError`  
C. `SyntaxError`  
D. `OSError`  
<details>
<summary>Answer</summary>
A. `ModuleNotFoundError` — Raised specifically when the module cannot be found.
</details>

---

### 4. What exception is raised when memory allocation fails?
A. `RuntimeError`  
B. `MemoryError`  
C. `SystemError`  
D. `OSError`  
<details>
<summary>Answer</summary>
B. `MemoryError` — Raised when an operation runs out of memory.
</details>

---

### 5. What will "2" + 2 raise?
A. `TypeError`  
B. `ValueError`  
C. `SyntaxError`  
D. `AttributeError`  
<details>
<summary>Answer</summary>
A. `TypeError` — Raised because a string cannot be added to an integer without conversion.
</details>

---

### 6. Which error occurs when you exceed the maximum recursion depth?
A. `RuntimeError`  
B. `RecursionError`  
C. `MemoryError`  
D. `OverflowError`  
<details>
<summary>Answer</summary>
B. `RecursionError` — Raised when the interpreter detects that the maximum recursion depth has been exceeded.
</details>

---

### 7. Which of these is a subclass of `LookupError`?
A. `IndexError`  
B. `TypeError`  
C. `SyntaxError`  
D. `NameError`  
<details>
<summary>Answer</summary>
A. `IndexError` — It is raised when a sequence subscript is out of range and is a subclass of `LookupError`.
</details>

---

### 8. Which exception does this code raise? `print(undefined_variable)`
A. `KeyError`  
B. `NameError`  
C. `AttributeError`  
D. `TypeError`  
<details>
<summary>Answer</summary>
B. `NameError` — Raised when a local or global name is not found.
</details>

---

### 9. What kind of exception is `StopIteration`?
A. A control flow exception  
B. A system exit exception  
C. A syntax error  
D. A lookup error  
<details>
<summary>Answer</summary>
A. A control flow exception — It signals the end of an iterator.
</details>

---

### 10. Which exception is raised when a Unicode encode operation fails?
A. `ValueError`  
B. `IOError`  
C. `UnicodeError`  
D. `TypeError`  
<details>
<summary>Answer</summary>
C. `UnicodeError` — Raised for encoding/decoding errors related to Unicode.
</details>

---

### 11. What exception is raised when a file or directory cannot be found?
A. `FileNotFoundError`  
B. `IOError`  
C. `OSError`  
D. `RuntimeError`  
<details>
<summary>Answer</summary>
A. `FileNotFoundError` — Raised when an attempt to open a file fails because the file does not exist.
</details>

---

### 12. Which exception is raised when trying to access a non-existent dictionary key?
A. `KeyError`  
B. `IndexError`  
C. `AttributeError`  
D. `ValueError`  
<details>
<summary>Answer</summary>
A. `KeyError` — Raised when a dictionary key is not found.
</details>

---

### 13. Which exception is triggered when using inconsistent indentation with tabs and spaces?
A. `SyntaxError`  
B. `IndentationError`  
C. `TabError`  
D. `TypeError`  
<details>
<summary>Answer</summary>
C. `TabError` — A subclass of `IndentationError`, raised for mixing tabs and spaces.
</details>

---

### 14. What is the base class for all built-in exceptions except system-exit exceptions?
A. `Exception`  
B. `BaseException`  
C. `RuntimeError`  
D. `SystemExit`  
<details>
<summary>Answer</summary>
A. `Exception` — It is the base class for all built-in exceptions except system-exit exceptions like `SystemExit`, `KeyboardInterrupt`.
</details>

---

### 15. What exception will `open('nofile.txt', 'r')` raise if the file does not exist?
A. `OSError`  
B. `IOError`  
C. `FileNotFoundError`  
D. `ValueError`  
<details>
<summary>Answer</summary>
C. `FileNotFoundError` — Raised when an open() call fails because the file doesn’t exist.
</details>

---

### 16. What exception will this code raise?
```python
my_list = [1, 2, 3]
print(my_list[5])
```
A. `KeyError`  
B. `IndexError`  
C. `AttributeError`  
D. `TypeError`  
<details>
<summary>Answer</summary>
B. `IndexError` — Raised when accessing an index outside the range of a list.
</details>

---

### 17. What exception will this code raise?
```python
def divide(a, b):
    return a / b

print(divide(10, 0))
```
A. `ArithmeticError`  
B. `ZeroDivisionError`  
C. `ValueError`  
D. `OverflowError`  
<details>
<summary>Answer</summary>
B. `ZeroDivisionError` — Raised when division or modulo by zero is attempted.
</details>

---

### 18. What exception will this code raise?
```python
class Base:
    def method(self):
        raise NotImplementedError("Must override method")

b = Base()
b.method()
```
A. `AttributeError`  
B. `TypeError`  
C. `NotImplementedError`  
D. `SyntaxError`  
<details>
<summary>Answer</summary>
C. `NotImplementedError` — Raised to indicate that a method is abstract and needs overriding.
</details>

---

### 19. What exception will this code raise?
```python
try:
    raise KeyboardInterrupt
except:
    print("Caught!")
```
A. It prints "Caught!"  
B. `KeyboardInterrupt` terminates the program  
C. `SystemExit`  
D. `ValueError`  
<details>
<summary>Answer</summary>
B. `KeyboardInterrupt` terminates the program — It is derived directly from `BaseException` and typically not caught by a bare `except`.
</details>

---

### 20. What exception will be raised by this code?
```python
"hello".foo()
```
A. `NameError`  
B. `AttributeError`  
C. `TypeError`  
D. `KeyError`  
<details>
<summary>Answer</summary>
B. `AttributeError` — Raised when attribute reference or assignment fails (no method `foo` in str).
</details>

---

### 21. What exception is raised when a float is passed to a function expecting an integer for indexing?
A. `ValueError`  
B. `TypeError`  
C. `IndexError`  
D. `AttributeError`  
<details>
<summary>Answer</summary>
B. `TypeError` — Indexes must be integers, so passing a float will raise this exception.
</details>

---

### 22. What kind of error will this code raise?  
```python
with open("file.txt") as f:
    content = f.read()
```
(Assuming `file.txt` does not exist.)  
A. `OSError`  
B. `FileNotFoundError`  
C. `IOError`  
D. `ValueError`  
<details>
<summary>Answer</summary>
B. `FileNotFoundError` — Raised when a file or directory is requested but doesn’t exist.
</details>

---

### 23. What exception is raised when the `next()` function is called on an exhausted iterator?
A. `StopIteration`  
B. `IndexError`  
C. `ValueError`  
D. `EOFError`  
<details>
<summary>Answer</summary>
A. `StopIteration` — Used to signal the end of iteration.
</details>

---

### 24. What exception does `eval('x === y')` raise in Python?
A. `SyntaxError`  
B. `NameError`  
C. `TypeError`  
D. `ValueError`  
<details>
<summary>Answer</summary>
A. `SyntaxError` — Python does not recognize `===` as valid syntax.
</details>

---

### 25. What exception is raised when attempting to divide by zero using the floor division operator `//`?
A. `ArithmeticError`  
B. `ValueError`  
C. `ZeroDivisionError`  
D. `TypeError`  
<details>
<summary>Answer</summary>
C. `ZeroDivisionError` — Raised by all types of division or modulo by zero, including `//`.
</details>

---

### 26. What is the output?

```python
# initialize the amount variable
try:
  amount = 10000

  if(amount>2999)
      print("You are eligible to purchase Dsa Self Paced")
except Exception:
  print("Something went wrong")
except SyntaxError:
  print("Syntax Error!")
except TypeError:
  print("Type Error")
```
<Details>
<summary>
Answer
</summary>
- Because SyntaxError is not caught during runtime — it is detected at compile time (i.e., when Python parses the code before running it).

So your code never enters the try block at all, because Python stops with a syntax error during parsing. Therefore, the try-except never even gets a chance to run.


</Details>

---

### 27. In Java, throw is used to explicitly raise an exception.In Python, ---------- is used to do the same thing.?
A. also `throw`  
B. `raise`  
C. `error`  
D. none of these  

<Details>
<summary>
Answer
</summary>
B. `raise`

</Details>

---  

### 28. if the function always raises an exception or runs indefinitely use ------------ return datatype:
A. `None`  
B. `null`  
C. `NoReturn`  
D. don't write return type 

<Details>
<summary>
Answer
</summary>
C. `NoReturn`


</Details>

---   

### 29. `NoReturn` majorly used:
A. for static analysis tool  
B. for readability  
C. same as `None`  
D. none of these    


<Details>
<summary>
Answer
</summary>
A. for static anlysis  tools   
(like mypy)


</Details>

---

### 30. what is the output?
``` python
try:
    print(var)
except NameError as e:
    print(e)
except TypeError:
  print(e)
except Exception as e:
  print(e)
```

A. NameError Block run  
B. TypeError Block run   
C. Generic Exception run  
D. try block run  
<Details>
<summary>
Output
</summary>
"NameError: name is not defined" printed

</Details>

### 31. What is the output of open("non_existent_file.txt")?
  A. FileNotFoundError
  B. FileExistsError
  C. FileCrashError
  D. other than file error  

<Details>
<summary>
Output
</summary>
A. FileNotFoundError

</Details>
