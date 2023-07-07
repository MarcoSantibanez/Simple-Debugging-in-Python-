# Simple-Debugging-in-Python-
Debugging in Python

At my organization I was tasked with helping my team with debugging some parts of code.

There are mainly three kinds of distinguishable errors in Python: *syntax errors*, *exceptions* and *logical errors*.

**Syntax** errors are similar to grammar or spelling errors in a Language. If there is such an error in your code, Python 
cannot start to execute your code. You get a clear error message stating what is wrong and what needs to be fixed.
Therefore, it is the easiest error type you can fix. Missing symbols (such as comma, bracket, colon), misspelling 
a keyword, having incorrect indentation are common syntax errors in Python.

**Exceptions** may occur in syntactically correct code blocks at run time. When Python cannot execute the requested action,
it terminates the code and raises an error message. Trying to read from a file which does not exist, performing operations
with incompatible types of variables, dividing a number by zero are common exceptions that raise an error in Python.
We must eliminate the syntax errors to run our Python code, while exceptions can be handled at runtime.

**Logical errors** are the most difficult errors to fix as they don’t crash your code and you don’t get any error message.
If you have logical errors, your code does not run as you expected. Using incorrect variable names, code that is not 
reflecting the algorithm logic properly, making mistakes on boolean operators will result in logical errors.

**First I was presented with the following syntax error:**

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/475d42a3-afbc-4129-b7e0-43f60f24d136)

Upon further examination of the code based on the output, I was made aware that there was a missing Colon operator **:** for the 
*For* loop to iterate correctly:

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/27e6bec3-a5bf-429a-93f5-745f634e8c1a)

A *for* loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string).
This is less like the for keyword in other programming languages, and works more like an iterator method as found 
in other object-orientated programming languages. With the for loop we can execute a set of statements, once for 
each item in a list, tuple, set etc.

After correcting the syntax error, I was tasked with looking at another part of the code that needed further debugging.
Another syntax error was presented in another part of the code that I was tasked with debugging. 

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/7dc0dd6f-7ad1-42ce-9f07-42e10e277f2f)

Upon further examination of the code based on the output, I was made aware that in the string list one of the names was not properly
placed in quotations to be stringed by adding them the code ran correctly free from errors:

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/57caa27c-9c56-4443-b331-9883e0b5f43b)

**Next I was presented with antoher syntax error:**

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/89518c4d-6989-4038-b937-b3e5ffcac78b)

Upon review I did notice that there was a missing parantheses at the end of the .upper() string function. 

~The *.upper()* method returns a string where all characters are in upper case.~

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/f2e99f02-2f1b-4bc5-bb00-2dd605d33561)

Next I was tasked with debugging another section of the code:

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/33011768-9093-4e90-9967-2e6fc56f0e24)

First correction needed was an invalid syntax. 

Then the print() function was not properly indented:

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/93f0969b-de3f-41fd-82ba-009c9c306043)

After correcting the indentation error the code ran correctly:

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/a42b53ab-8906-4dc9-bfc2-7acc1c4ebf45)

There was still an exception error that needed correcting for that I backtraced the output of code to find the error:

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/dd7ccb6a-9732-4d67-8a3e-95e3c3bb2d7f)

Even if a statement or expression is syntactically correct, it may cause an error when an attempt is made to execute it. 
Errors detected during execution are called exceptions and are not unconditionally fatal.

Since my team wanted the name of the user to be shown I added the above in the code *, username ,*. 

My team wanted my to add an else statement. 

Upon entering the else statement I was presented with a logical error:

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/916209bb-fb93-40b4-b1a9-b84a33b5d4c5)

A logical error occurs in Python when the code runs without any syntax or runtime errors but produces incorrect
results due to flawed logic in the code. These types of errors are often caused by incorrect assumptions, 
an incomplete understanding of the problem, or the incorrect use of algorithms or formulas.

For fixing the above error I added break statements:


![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/da9c02d9-d9d5-47bf-81e8-ff93f8e65b4e)
![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/d0f5e849-8bb9-41b6-ac7e-2cd8d610b0f4)

![image](https://github.com/MarcoSantibanez/Simple-Debugging-in-Python-/assets/138132151/cf338e07-e04b-4fb5-94d9-e395e8a4e4cf)


In Python, break allows you to exit a loop when an external condition is met. Normal program execution resumes at the next statement. You can use a break statement with both for loops and while loops. In a nested loop, break will stop execution of the innermost loop. The flow of the program resumes at the next line of code immediately after the block.


Summary: 

**I was able to succesfully debug three types of errors that included *syntax*, *logical* and *exception* errors.**  















