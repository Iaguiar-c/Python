# Writing Your First Python Code       

## Say 'Hello' to the world in Python

When learning a new programming language, it is customary to start with an "hello world" example. As simple as it is, this one line of code will ensure that we know how to print a string in output and how to execute code within cells in a notebook.

<hr/>
<div class="alert alert-success alertsuccess" style="margin-top: 20px">
[Tip]: To execute the Python code in the code cell below, click on the cell to select it and press <kbd>Shift</kbd> + <kbd>Enter</kbd>.
</div>
<hr/>

# Try your first Python output

print('Hello, Python!')
After executing the cell above, you should see that Python prints <code>Hello, Python!</code>. Congratulations on running your first Python code!

<hr/>
<div class="alert alert-success alertsuccess" style="margin-top: 20px">
    [Tip:] <code>print()</code> is a function. You passed the string <code>'Hello, Python!'</code> as an argument to instruct Python on what to print.
</div>
<hr/>

### What version of Python are we using?

<p>
    Python 2 is no longer in use, as it officially reached end-of-life on January 1, 2020. The Python community and most major libraries have fully adopted Python 3, which is now the standard for all development and learning.
</p>
<p>
    In this course, we use Python 3 exclusively in all our labs. How do we know that our notebook is executed by a Python 3 runtime?
</p>
<p>
    We can ask Python directly and obtain a detailed answer. Try executing the following code:
</p>

# Check the Python Version

import sys
print(sys.version)
<hr/>
<div class="alert alert-success alertsuccess" style="margin-top: 20px">
    [Tip:] <code>sys</code> is a built-in module that contains many system-specific parameters and functions, including the Python version in use. Before using it, we must explictly <code>import</code> it.
</div>
<hr/>

### Writing comments in Python

<p>
    In addition to writing code, note that it's always a good idea to add comments to your code. It will help others understand what you were trying to accomplish (the reason why you wrote a given snippet of code). Not only does this help <strong>other people</strong> understand your code, it can also serve as a reminder <strong>to you</strong> when you come back to it weeks or months later.</p>

<p>
    To write comments in Python, use the number symbol <code>#</code> before writing your comment. When you run your code, Python will ignore everything past the <code>#</code> on a given line.
</p>

# Practice on writing comments

print('Hello, Python!') # This line prints a string
# print("Hi")
<p>
    After executing the cell above, you should notice that <code>This line prints a string</code> did not appear in the output, because it was a comment (and thus ignored by Python).
</p>
<p>
    The second line was also not executed because <code>print('Hi')</code> was preceded by the number sign (<code>#</code>) as well! Since this isn't an explanatory comment from the programmer, but an actual line of code, we might say that the programmer <em>commented out</em> that second line of code.
</p>

<h3 id="errors">Errors in Python</h3>

<p>Everyone makes mistakes. For many types of mistakes, Python will tell you that you have made a mistake by giving you an error message. It is important to read error messages carefully to really understand where you made a mistake and how you may go about correcting it.</p>
<p>For example, if you spell <code>print</code> as <code>frint</code>, Python will display an error message. Give it a try:</p>

# Print string as error message

frint("Hello, Python!")
<p>The error message tells you: 
<ol>
    <li>where the error occurred (more useful in large notebook cells or scripts), and</li> 
    <li>what kind of error it was (NameError)</li> 
</ol>
<p>Here, Python attempted to run the function <code>frint</code>, but could not determine what <code>frint</code> is since it's not a built-in function and it has not been previously defined by us either.</p>

<p>
    You'll notice that if we make a different type of mistake, by forgetting to close the string, we'll obtain a different error (i.e., a <code>SyntaxError</code>). Try it below:
</p>

# Try to see built-in error message

print("Hello, Python!)
### Does Python know about your error before it runs your code?

Python is what is called an <em>interpreted language</em>. Compiled languages examine your entire program at compile time, and are able to warn you about a whole class of errors prior to execution. In contrast, Python interprets your script line by line as it executes it. Python will stop executing the entire program when it encounters an error (unless the error is expected and handled by the programmer, a more advanced subject that we'll cover later on in this course).

Try to run the code in the cell below and see what happens:

# Print string and error to see the running order

print("This will be printed")
frint("This will cause an error")
print("This will NOT be printed")
### Exercise: Your First Program

<p>Generations of programmers have started their coding careers by simply printing "Hello, world!". You will be following in their footsteps.</p>
<p>In the code cell below, use the <code>print()</code> function to print out the phrase: <code>Hello, world!</code></p>

# Write your code below. Don't forget to press Shift+Enter to execute the cell
print("Hello, world!")
<details><summary>Click here for the solution</summary>

```python
print("Hello, world!")

```

</details>

<p>Now, let's enhance your code with a comment. In the code cell below, print out the phrase: <code>Hello, world!</code> and comment it with the phrase <code>Print the traditional hello world</code> all in one line of code.</p>

# Write your code below. Don't forget to press Shift+Enter to execute the cell
print("Hello, world!") #Print the traditional hello world
<details><summary>Click here for the solution</summary>

```python
print("Hello, world!") # Print the traditional hello world

```

</details>

<p>What is the value of <code>z</code> where <code>z = 2 + 15</code>?</p>

# Write your code below. Don't forget to press Shift+Enter to execute the cell
print("17")
<details><summary>Click here for the solution</summary>

```python
17

```

</details>

<hr>

<p>Congratulations, you have completed your first lesson and hands-on lab in Python.
<hr>