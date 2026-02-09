## What are Strings?

The following example shows a string contained within 2 quotation marks:

# Use quotation marks for defining string

"The BodyGuard"
We can also use single quotation marks:

# Use single quotation marks for defining string

'The BodyGuard'
A string can be a combination of spaces and digits:

# Digitals and spaces in string

'1 2 3 4 5 6 '
A string can also be a combination of special characters :

# Special characters in string

'@#2_#]&*^%$'
We can print our string using the print statement:

# Print the string

print("hello!")
We can bind or assign a string to another variable:

# Assign string to variable

name = "The BodyGuard"
name
<hr>

## Indexing

It is helpful to think of a string as an ordered sequence. Each element in the sequence can be accessed using an index represented by the array of numbers:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/xwKqWxQWBL47h718d3BLzw/IMG1.png" width="600" align="center">

The first index can be accessed as follows:

<hr/>
<div class="alert alert-success alertsuccess" style="margin-top: 20px">
[Tip]: Because indexing starts at 0, it means the first index is on the index 0.
</div>
<hr/>

# Print the first element in the string

print(name[0])
We can access index 6:

# Print the element on index 6 in the string

print(name[6])
Moreover, we can access the 10th index:

# Print the element on the 10th index in the string

print(name[10])
### Negative Indexing

We can also use negative indexing with strings:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/VAdKOVUWpsM7hC7CjWmEdQ/IMG2.png" width="600" align="center">

Negative index can help us to count the element from the end of the string.

The last element is given by the index -1:

# Print the last element in the string

print(name[-1])
The first element can be obtained by  index -11:

# Print the first element in the string

print(name[-13])
We can find the number of characters in a string by using <code>len</code>, short for length:

# Find the length of string

len("The BodyGuard")
### Slicing

We can obtain multiple characters from a string using slicing, we can obtain the 0 to 4th and 8th to the 12th element:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/Ph9xvvIvaf-krPI-qoaZ2Q/IMG3.png" width="600" align="center">

<hr/>
<div class="alert alert-success alertsuccess" style="margin-top: 20px">
[Tip]: When taking the slice, the first number means the index (start at 0), and the second number means the length from the index to the last element you want (start at 1)
</div>
<hr/>

# Take the slice on variable name with only index 0 to index 3

name[0:4]
# Take the slice on variable name with only index 8 to index 11

name[8:12]
### Stride

We can also input a stride value as follows, with the '2' indicating that we are selecting every second variable:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/SaORQ3bZLArgeix_9-jjRQ/IMG4.png" width="600" align="center">

# Get every second element, starting with the index 0. The elments on index 0, 2, 4 ...

name[::2]
We can also incorporate slicing  with the stride. In this case, we select the first five elements and then use the stride:

# Get every second element in the range from index 0 to index 4

name[0:5:2]
### Concatenate Strings

We can concatenate or combine strings by using the addition symbols, and the result is a new string that is a combination of both:

# Concatenate two strings

statement = name + " is the best album"
statement
To replicate values of a string we simply multiply the string by the number of times we would like to replicate it. In this case, the number is three. The result is a new string, and this new string consists of three copies of the original string:

# Print the string for 3 times

3 * "The BodyGuard"
You can create a new string by setting it to the original variable. Concatenated  with a new string, the result is a new string that changes from The BodyGuard to “The BodyGuard is the best album".

# Concatenate strings

name = "The BodyGuard"
name = name + " is the best album"
name
<hr>

## Escape Sequences

Back slashes represent the beginning  of escape sequences. Escape sequences represent strings that may be difficult to input. For example, back slash "n" represents a new line. The output is given by a new line after the back slash "n" is encountered:

# New line escape sequence

print(" The BodyGuard\n is the best album" )
Similarly, back slash  "t" represents a tab:

# Tab escape sequence

print(" The BodyGuard \t is the best album" )
If you want to place a back slash in your string, use a double back slash:

# Include back slash in string

print(" The BodyGuard \\ is the best album" )
We can also place an "r" before the string to display the backslash:

# r will tell python that string will be display as raw string

print(r" The BodyGuard \ is the best album" )
<hr>

## String Manipulation Operations

There are many string operation methods in Python that can be used to manipulate the data. We are going to use some basic string operations on the data.

Let's try with the method <code>upper</code>; this method converts lower case characters to upper case characters:

# Convert all the characters in string to upper case

a = "Thriller is the sixth studio album"
print("before upper:", a)
b = a.upper()
print("After upper:", b)
The method <code>replace</code> replaces a segment of the string, i.e. a substring  with a new string. We input the part of the string we would like to change. The second argument is what we would like to exchange the segment with, and the result is a new string with the segment changed:

# Replace the old substring with the new target substring is the segment has been found in the string

a = "The BodyGuard is the best album"
b = a.replace('BodyGuard', 'Janet')
b
The method <code>find</code> finds a sub-string. The argument is the substring you would like to find, and the output is the first index of the sequence. We can find the sub-string <code>he</code> or <code>Guard<code>.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/eK6pP3xD4kLWk2vri9KA5A/IMG5.png" width="600" align="center">

# Find the substring in the string. Only the index of the first elment of substring in string will be the output

name = "The BodyGuard"
name.find('he')
# Find the substring in the string.

name.find('Guard')
If the  sub-string is not in the string then the output is a negative one. For example, the string 'Jasdfasdasdf' is not a substring:

# If cannot find the substring in the string

name.find('Jasdfasdasdf')
The method <code>Split</code> splits the string at the specified separator, and returns a list.

**Syntax**

<code>string.split(separator, maxsplit)</code>

**Parameters**
- separator (optional): This is the delimiter at which the string will be split. If not provided, the default separator is any whitespace.
- maxsplit (optional): This specifies the maximum number of splits to perform. If not provided, there is no limit on the number of splits.

**Return Value**:

The method returns a list of substrings.

#Split the substring into list
name = "The BodyGuard"
split_string = (name.split())
split_string
<hr>

## RegEx

In Python, RegEx (short for Regular Expression) is a tool for matching and handling strings. 

This RegEx module provides several functions for working with regular expressions, including <code>search, split, findall,</code> and <code>sub</code>. 

Python provides a built-in module called <code>re</code>, which allows you to work with regular expressions. 
First, import the <code>re</code> module

import re
The search() function searches for specified patterns within a string. Here is an example that explains how to use the search() function to search for the word "Body" in the string "The BodyGuard is the best".

s1 = "The BodyGuard is the best album"

# Define the pattern to search for
pattern = r"Body"

# Use the search() function to search for the pattern in the string
result = re.search(pattern, s1)

# Check if a match was found
if result:
    print("Match found!")
else:
    print("Match not found.")

Regular expressions (RegEx) are patterns used to match and manipulate strings of text. There are several special sequences in RegEx that can be used to match specific characters or patterns.

| Special Sequence | Meaning                 | 	Example             |
| -----------  | ----------------------- | ----------------------|
| \d|Matches any digit character (0-9)|"123" matches "\d\d\d"|
|\D|Matches any non-digit character|"hello" matches "\D\D\D\D\D"|
|\w|Matches any word character (a-z, A-Z, 0-9, and _)|"hello_world" matches "\w\w\w\w\w\w\w\w\w\w\w"|
|\W|Matches any non-word character|	"@#$%" matches "\W\W\W\W"|
|\s|Matches any whitespace character (space, tab, newline, etc.)|"hello world" matches "\w\w\w\w\w\s\w\w\w\w\w"|
|\S|Matches any non-whitespace character|"hello_world" matches "\S\S\S\S\S\S\S\S\S\S\S"|
|\b|Matches the boundary between a word character and a non-word character|"cat" matches "\bcat\b" in "The cat sat on the mat"|
|\B|Matches any position that is not a word boundary|"cat" matches "\Bcat\B" in "category" but not in "The cat sat on the mat"|

Special Sequence Examples:

A simple example of using the <code>\d</code> special sequence in a regular expression pattern with Python code:

pattern = r"\d\d\d\d\d\d\d\d\d\d"  # Matches any ten consecutive digits
text = "My Phone number is 1234567890"
match = re.search(pattern, text)

if match:
    print("Phone number found:", match.group())
else:
    print("No match")
The match.group() method is used in Python's re module to retrieve the part of the string where the regular expression pattern matched. Here's a detailed explanation:

**Purpose**
- Extract Matched Text: match.group() returns the exact substring that matched the pattern.
 
**Usage**
- When you use functions like re.search() or re.match(), they return a match object if the pattern is found. You can then use match.group() to get the matched text.

Here `match.group()` retrieves the substring 1234567890 from the text, which is the part that matched the pattern.

The regular expression pattern is defined as r"\d\d\d\d\d\d\d\d\d\d", which uses the \d special sequence to match any digit character (0-9), and the \d sequence is repeated ten times to match ten consecutive digits

A simple example of using the <code>\W</code> special sequence in a regular expression pattern with Python code:

pattern = r"\W"  # Matches any non-word character
text = "Hello, world!"
matches = re.findall(pattern, text)

print("Matches:", matches)
The regular expression pattern is defined as r"\W", which uses the \W special sequence to match any character that is not a word character (a-z, A-Z, 0-9, or _). The string we're searching for matches in is "Hello, world!".

The <code>findall()</code> function finds all occurrences of a specified pattern within a string.

s2 = "The BodyGuard is the best album of 'Whitney Houston'."


# Use the findall() function to find all occurrences of the "st" in the string
result = re.findall("st", s2)

# Print out the list of matched words
print(result)

A regular expression's <code>split()</code> function splits a string into an array of substrings based on a specified pattern.

# Use the split function to split the string by the "\s"
split_array = re.split(r"\s", s2)

# The split_array contains all the substrings, split by whitespace characters
print(split_array)
Here's a detailed explanation: 

<code>re.split("\s", s2)</code>:

**re.split**: This function splits a string by the occurrences of a pattern.
- **r"\s"**: This is a regular expression pattern that matches any whitespace character (spaces, tabs, newlines, etc.).
- **s2**: This is the string that you want to split.

The <code>sub</code> function of a regular expression in Python is used to replace all occurrences of a pattern in a string with a specified replacement.

# Define the regular expression pattern to search for
pattern = r"Whitney Houston"

# Define the replacement string
replacement = "legend"

# Use the sub function to replace the pattern with the replacement string
new_string = re.sub(pattern, replacement, s2, flags=re.IGNORECASE) # re.IGNORECASE makes the search case-insensitive, so it matches "Whitney Houston" in any letter case

# The new_string contains the original string with the pattern replaced by the replacement string
print(new_string) 
<hr>

<h2 id="quiz">Quiz on Strings</h2>

What is the value of the variable <code>a</code> after the following code is executed?

# Write your code below and press Shift+Enter to execute 

a = "1"
a
<details><summary>Click here for the solution</summary>

```python
"1"

```

</details>

What is the value of the variable <code>b</code> after the following code is executed?

# Write your code below and press Shift+Enter to execute

b = "2"
b
<details><summary>Click here for the solution</summary>

```python
"2"

```

</details>

What is the value of the variable <code>c</code> after the following code is executed?

# Write your code below and press Shift+Enter to execute 

c = a + b
c
<details><summary>Click here for the solution</summary>

```python
"12"

```

</details>

<hr>

Consider the variable <code>d</code> use slicing to print out the first three elements:

# Write your code below and press Shift+Enter to execute

d = "ABCDEFG"
print(d[:3])
<details><summary>Click here for the solution</summary>

```python
print(d[:3]) 

# or 

print(d[0:3])

```

</details>

<hr>

Use a stride value of 2 to print out every second character of the string <code>e</code>:

# Write your code below and press Shift+Enter to execute

e = 'clocrkr1e1c1t'
print(e[::2])
<details><summary>Click here for the solution</summary>

```python
print(e[::2])

```

</details>

<hr>

Print out a backslash:

# Write your code below and press Shift+Enter to execute
print(r"\\")
print(r"\\")
<details><summary>Click here for the solution</summary>

```python
print("\\\\\\\\\\\\\\\\")

or

print(r"\\")

```

</details>

<hr>

Convert the variable <code>f</code> to uppercase:

# Write your code below and press Shift+Enter to execute

f = "You are wrong"
f.upper()
<details><summary>Click here for the solution</summary>

```python
f.upper()

```

</details>

Convert the variable <code>f2</code> to lowercase:

# Write your code below and press Shift+Enter to execute
f2="YOU ARE RIGHT"
f2.lower()
<details><summary>Click here for the solution</summary>

```python
f2.lower()

```

</details>

<hr>

Consider the variable <code>g</code>, and find the first index of the sub-string <code>snow</code>:

# Write your code below and press Shift+Enter to execute

g = "Mary had a little lamb Little lamb, little lamb Mary had a little lamb \
Its fleece was white as snow And everywhere that Mary went Mary went, Mary went \
Everywhere that Mary went The lamb was sure to go"
g.find("snow")
<details><summary>Click here for the solution</summary>

```python
g.find("snow")

```

</details>

In the variable <code>g</code>, replace the sub-string <code>Mary</code> with <code>Bob</code>:

# Write your code below and press Shift+Enter to execute
g.replace
<details><summary>Click here for the solution</summary>

```python
g.replace("Mary", "Bob")

```

</details>

In the variable <code>g</code>, replace the sub-string <code>,</code> with <code>.</code>:

# Write your code below and press Shift+Enter to execute
<details><summary>Click here for the solution</summary>

```python
g.replace(',','.')

```

</details>

In the variable <code>g</code>, split the substring to list:

# Write your code below and press Shift+Enter to execute
<details><summary>Click here for the solution</summary>

```python
g.split()

```

</details>

In the string <code>s3</code>, find whether the digit is present or not using the <code>\d</code> and <code>search() </code>function:

s3 = "House number- 1105"
# Write your code below and press Shift+Enter to execute
<details><summary>Click here for the solution</summary>

```python
# Use the search() function to search for the "\d" in the string
result = re.search(r"\d", s3)

# Check if a match was found
if result:
    print("Digit found")
else:
    print("Digit not found.")
```

</details>

In the string <code>str1</code>, replace the sub-string <code>fox</code> with <code>bear</code> using <code>sub() </code>function:

str1= "The quick brown fox jumps over the lazy dog."

# Write your code below and press Shift+Enter to execute

<details><summary>Click here for the solution</summary>

```python
# Use re.sub() to replace "fox" with "bear"
new_str1 = re.sub(r"fox", "bear", str1)

print(new_str1)
```

</details>

In the string <code>str2</code> find all the occurrences of <code>woo</code> using <code>findall()</code> function:

str2= "How much wood would a woodchuck chuck, if a woodchuck could chuck wood?"

# Write your code below and press Shift+Enter to execute

<details><summary>Click here for the solution</summary>

```python
# Use re.findall() to find all occurrences of "woo"
matches = re.findall(r"woo", str2)

print(matches)
```

</details>

<hr>
<h2>The last exercise!</h2>
<p>Congratulations, you have completed your first lesson and hands-on lab in Python.
<hr>