## Expressions and Variables

### Expressions

<p>Expressions in Python can include operations among compatible types (e.g., integers and floats). For example, basic arithmetic operations like adding multiple numbers:</p>

# Addition operation expression

43 + 60 + 16 + 41
<p>We can perform subtraction operations using the minus operator. In this case the result is a negative number:</p>

# Subtraction operation expression

50 - 60
<p>We can do multiplication using an asterisk:</p>

# Multiplication operation expression

5 * 5
<p>We can also perform division with the forward slash:

# Division operation expression

25 / 5
# Division operation expression

25 / 6
<p>As seen in the quiz above, we can use the double slash for integer division, where the result is rounded down to the nearest integer:

# Integer division operation expression

25 // 5
# Integer division operation expression

25 // 6
<p>Let's write an expression that calculates how many hours there are in 160 minutes:

# Write your code below. Don't forget to press Shift+Enter to execute the cell
160//60 
<p>Python follows well accepted mathematical conventions when evaluating mathematical expressions. In the following example, Python adds 30 to the result of the multiplication (i.e., 120).

# Mathematical expression

30 + 2 * 60
<p>And just like mathematics, expressions enclosed in parentheses have priority. So the following multiplies 32 by 60.

# Mathematical expression

(30 + 2) * 60
### Variables

<p>Just like with most programming languages, we can store values in <i>variables</i>, so we can use them later on. For example:</p>

# Store value into variable

x = 43 + 60 + 16 + 41
<p>To see the value of <code>x</code> in a Notebook, we can simply place it on the last line of a cell:</p>

# Print out the value in variable

x
<p>We can also perform operations on <code>x</code> and save the result to a new variable:</p>

# Use another variable to store the result of the operation between variable and value

y = x / 60
y
<p>If we save a value to an existing variable, the new value will overwrite the previous value:</p>

# Overwrite variable with new value

x = x / 60
x
<p>It's a good practice to use meaningful variable names, so you and others can read the code and understand it more easily:</p>

# Name the variables meaningfully

total_min = 43 + 42 + 57 # Total length of albums in minutes
total_min
# Name the variables meaningfully

total_hours = total_min / 60 # Total length of albums in hours 
total_hours
<p>In the cells above we added the length of three albums in minutes and stored it in <code>total_min</code>. We then divided it by 60 to calculate total length <code>total_hours</code> in hours. You can also do it all at once in a single expression, as long as you use parenthesis to add the albums length before you divide, as shown below.</p>

# ComplicateD expression

total_hours = (43 + 42 + 57) / 60  # Total hours in a single expression
total_hours
<p>If you'd rather have total hours as an integer, you can of course replace the floating point division with integer division (i.e., <code>//</code>).</p>

### Exercise: Expressions in Python

Write an expression to add 30 and 20 and subtract 40

# Write your code below. Don't forget to press Shift+Enter to execute the cell
30+20-40
<details><summary>Click here for the solution</summary>

```python

30+20-40
# This will print 10

```

</details>

Write an expression to subtract 5 from 55 and divide the result by 10

# Write your code below. Don't forget to press Shift+Enter to execute the cell
x = 55 - 5
y = x / 10
y
<details><summary>Click here for the solution</summary>

```python

(55-5)/10
# This will print 5.0

```

</details>

Write an expression to multiply 6 with 10 and divide the result by 12

# Write your code below. Don't forget to press Shift+Enter to execute the cell

<details><summary>Click here for the solution</summary>

```python

(6*10)/12
# This will print 5.0

```

</details>

### Exercise: Variables in Python

<p>What is the value of <code>x</code> where <code>x = 3 + 2 * 2</code></p>

# Write your code below. Don't forget to press Shift+Enter to execute the cell

<details><summary>Click here for the solution</summary>

```python
x = 3 + 2 * 2
x
# This will print 7

```

</details>

<p>What is the value of <code>y</code> where <code>y = (3 + 2) * 2</code>?</p>

# Write your code below. Don't forget to press Shift+Enter to execute the cell

<details><summary>Click here for the solution</summary>

```python

y = (3 + 2) * 2
y
# This will print 10

```

</details>

<p>What is the value of <code>z</code> where <code>z = x + y</code>?</p>

# Write your code below. Don't forget to press Shift+Enter to execute the cell

<details><summary>Click here for the solution</summary>

```python

z = x+y 
z
# This will print 17

```

</details>

<hr>
<p>Congratulations, you have completed your hands-on lab on Expressions and Variables in Python.
<hr>