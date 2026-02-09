## Types of objects in Python

<p>Python is an object-oriented language. There are many different types of objects in Python. Let's start with the most common object types: <i>strings</i>, <i>integers</i> and <i>floats</i>. Anytime you write words (text) in Python, you're using <i>character strings</i> (strings for short). The most common numbers, on the other hand, are <i>integers</i> (e.g. -1, 0, 100) and <i>floats</i>, which represent real numbers (e.g. 3.14, -42.0).</p>

<a align="center">
    <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%201/images/TypesObjects.png" width="600">
</a>

<p>The following code cells contain some examples.</p>

# Integer

11
# Float

2.14
# String

"Hello, Python 101!"
<p>You can get Python to tell you the type of an expression by using the built-in <code>type()</code> function. You'll notice that Python refers to integers as <code>int</code>, floats as <code>float</code>, and character strings as <code>str</code>.</p>

# Type of 12

type(12)
# Type of 2.14

type(2.14)
# Type of "Hello, Python 101!"

type("Hello, Python 101!")
<p>In the code cell below, use the <code>type()</code> function to check the object type of <code>12.0</code>.

# Write your code below. Don't forget to press Shift+Enter to execute the cell
type(12.0)
<details><summary>Click here for the solution</summary>

```python
type(12.0)

```

</details>

### Integers

<p>Here are some examples of integers. Integers can be negative or positive numbers:</p>

<a align="center">
    <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%201/images/TypesInt.png" width="600">
</a>

<p>We can verify this is the case by using, you guessed it, the <code>type()</code> function:

# Print the type of -1

type(-1)
# Print the type of 4

type(4)
# Print the type of 0

type(0)
### Floats

<p>Floats represent real numbers; they are a superset of integer numbers but also include "numbers with decimals". There are some limitations when it comes to machines representing real numbers, but floating point numbers are a good representation in most cases. You can learn more about the specifics of floats for your runtime environment, by checking the value of <code>sys.float_info</code>. This will also tell you what's the largest and smallest number that can be represented with them.</p>

<p>Once again, can test some examples with the <code>type()</code> function:

# Print the type of 1.0

type(1.0) # Notice that 1 is an int, and 1.0 is a float
# Print the type of 0.5

type(0.5)
# Print the type of 0.56

type(0.56)
# System settings about float type
import sys
sys.float_info
### Converting from one object type to a different object type

<p>You can change the type of the object in Python; this is called typecasting. For example, you can convert an <i>integer</i> into a <i>float</i> (e.g. 2 to 2.0).</p>
<p>Let's try it:</p>

# Verify that this is an integer

type(2)
#### Converting integers to floats
<p>Let's cast integer 2 to float:</p>

# Convert 2 to a float

float(2)
# Convert integer 2 to a float and check its type

type(float(2))
<p>When we convert an integer into a float, we don't really change the value (i.e., the significand) of the number. However, if we cast a float into an integer, we could potentially lose some information. For example, if we cast the float 1.1 to integer we will get 1 and lose the decimal information (i.e., 0.1):</p>

# Casting 1.1 to integer will result in loss of information

int(1.1)
<h4>Converting from strings to integers or floats</h4>

<p>Sometimes, we can have a string that contains a number within it. If this is the case, we can cast that string that represents a number into an integer using <code>int()</code>:</p>

# Convert a string into an integer

int('1')
<p>But if you try to do so with a string that is not a perfect match for a number, you'll get an error. Try the following:</p>

# Convert a string into an integer with error

int('1 or 2 people')
<p>You can also convert strings containing floating point numbers into <i>float</i> objects:</p>

# Convert the string "1.2" into a float

float('1.2')
<hr/>
<div class="alert alert-success alertsuccess" style="margin-top: 20px">
    [Tip:] Note that strings can be represented with single quotes (<code>'1.2'</code>) or double quotes (<code>"1.2"</code>), but you can't mix both (e.g., <code>"1.2'</code>).
</div>
<hr/>

<h4>Converting numbers to strings</h4>

<p>If we can convert strings to numbers, it is only natural to assume that we can convert numbers to strings, right?</p>

# Convert an integer to a string

str(1)

<p>And there is no reason why we shouldn't be able to make floats into strings as well:</p> 

# Convert a float to a string

str(1.2)
### Boolean data type

<p><i>Boolean</i> is another important type in Python. An object of type <i>Boolean</i> can take on one of two values: <code>True</code> or <code>False</code>:</p>

# Value true

True
<p>Notice that the value <code>True</code> has an uppercase "T". The same is true for <code>False</code> (i.e. you must use the uppercase "F").</p>

# Value false

False
<p>When you ask Python to display the type of a boolean object it will show <code>bool</code> which stands for <i>boolean</i>:</p> 

# Type of True

type(True)
# Type of False

type(False)
<p>We can cast boolean objects to other data types. If we cast a boolean with a value of <code>True</code> to an integer or float we will get a one. If we cast a boolean with a value of <code>False</code> to an integer or float we will get a zero. Similarly, if we cast a 1 to a Boolean, you get a <code>True</code>. And if we cast a 0 to a Boolean we will get a <code>False</code>. Let's give it a try:</p> 

# Convert True to int

int(True)
# Convert 1 to boolean

bool(1)
# Convert 0 to boolean

bool(0)
# Convert True to float

float(True)
### Exercise: Types

<p>What is the data type of the result of: <code>6 / 2</code>?</p>

# Write your code below. Don't forget to press Shift+Enter to execute the cell
type(6/2)
<details><summary>Click here for the solution</summary>

```python
type(6/2) # float

```

</details>

<p>What is the type of the result of: <code>6 // 2</code>? (Note the double slash <code>//</code>.)</p>

# Write your code below. Don't forget to press Shift+Enter to execute the cell
type(6//2)
<details><summary>Click here for the solution</summary>

```python
type(6//2) # int, as the double slashes stand for integer division 

```

</details>

What is the type of the result of: <code>"Hello, World!"</code>

# Write your code below. Don't forget to press Shift+Enter to execute the cell
type('Hello, world!')
<details><summary>Click here for the solution</summary>

```python

type("Hello, World!") 

```

</details>

<hr>

What is the type of the result of: <code>"hello" == "world"</code>

# Write your code below. Don't forget to press Shift+Enter to execute the cell
type("hello" == "world")
<details><summary>Click here for the solution</summary>

```python

type("hello" == "world")  

```

</details>

Write the code to convert the following number representing employeeid **"1001"** to an integer

# Write your code below. Don't forget to press Shift+Enter to execute the cell
int
<details><summary>Click here for the solution</summary>

```python

int("1001")

```

</details>

Write the code to convert this number representing financial value **"1234.56"** to a floating point number

# Write your code below. Don't forget to press Shift+Enter to execute the cell

<details><summary>Click here for the solution</summary>

```python

float("1234.56")

```

</details>

Write the code to convert this phone number **123-456-7890** to a string

# Write your code below. Don't forget to press Shift+Enter to execute the cell
<details><summary>Click here for the solution</summary>

```python

str("123-456-7890")

```

</details>

<hr>

<p>Congratulations, you have completed your hands-on lab on Types in Python.
<hr>