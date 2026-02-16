## Loops

### Range

Sometimes, you might want to repeat a given operation many times. Repeated executions like this are performed by <b>loops</b>. We will look at two types of loops, <code>for</code> loops and <code>while</code> loops.

Before we discuss loops lets discuss the <code>range</code> object. It is helpful to think of the range object as an ordered list. For now, let's look at the simplest case. If we would like to generate an object that contains elements ordered from 0 to 2 we simply use the following command:

# Use the range

range(3)
<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/range.PNG" width="300">

***NOTE: While in Python 2.x it returned a list as seen in video lessons, in 3.x it returns a range object.***

### What is <code>for</code> loop?

The <code>for</code> loop enables you to execute a code block multiple times. For example, you would use this if you would like to print out every element in a list.\
Let's try to use a <code>for</code> loop to print all the years presented in the list <code>dates</code>:

This can be done as follows:

# For loop example

dates = [1982,1980,1973]
N = len(dates)

for i in range(N):
    print(dates[i])     
The code in the indent is executed <code>N</code> times, each time the value of <code>i</code> is increased by 1 for every execution. The statement executed is to <code>print</code> out the value in the list at index <code>i</code> as shown here:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/f3bJb12CNd053xJfk1wU2g/LoopsForRangee.gif" width="800">

In this example we can print out a sequence of numbers from 0 to 7:

# Example of for loop

for i in range(0, 8):
    print(i)
In Python we can directly access the elements in the list as follows:

# Exmaple of for loop, loop through list

for year in dates:  
    print(year)   
For each iteration, the value of the variable <code>year</code> behaves like the value of <code>dates\[i]</code> in the  first example:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/LoopsForList.gif" width="800">

We can change the elements in a list:

# Use for loop to change the elements in list

squares = ['red', 'yellow', 'green', 'purple', 'blue']

for i in range(0, 5):
    print("Before square ", i, 'is',  squares[i])
    squares[i] = 'white'
    print("After square ", i, 'is',  squares[i])
We can access the index and the elements of a list as follows:

# Loop through the list and iterate on both index and element value

squares=['red', 'yellow', 'green', 'purple', 'blue']

for i, square in enumerate(squares):
    print(i, square)
### What is <code>while</code> loop?

As you can see, the <code>for</code> loop is used for a controlled flow of repetition. However, what if we don't know when we want to stop the loop? What if we want to keep executing a code block until a certain condition is met? The <code>while</code> loop exists as a tool for repeated execution based on a condition. The code block will keep being executed until the given logical condition returns a **False** boolean value.

Let’s say we would like to iterate through list <code>dates</code> and stop at the year 1973, then print out the number of iterations. This can be done with the following block of code:

# While Loop Example

dates = [1982, 1980, 1973, 2000]

i = 0
year = dates[0]

while(year != 1973):    
    print(year)
    i = i + 1
    year = dates[i]
    

print("It took ", i ,"repetitions to get out of loop.")
A while loop iterates merely until the condition in the argument is not  met, as shown in the following figure:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/LoopsWhile.gif" width="650">

<hr>

## Controlling Loop Execution with <code>break</code> and <code>continue</code>

### The <code>break</code> statement

The <code>break</code> statement immediately terminates the loop it appears in, regardless of the loop’s condition.
It’s commonly used when a specific condition is met and no further iterations are needed.

Example 1: Using <code>break</code> in a <code>for</code> loop

for num in range(1, 10):
    if num == 5:
        print("Breaking the loop at:", num)
        break
    print(num)

Note: The loop stops as soon as num equals 5.

### The <code>continue</code> statement

The <code>continue</code> statement skips the current iteration and moves to the next one in the loop.
It’s used when you want to ignore certain conditions but continue looping.

Example 2: Using <code>continue</code> in a <code>for</code> loop

for num in range(1, 6):
    if num == 3:
        continue
    print(num)
Note: The number 3 is skipped, but the loop continues with the remaining iterations.

Example 3: Using <code>break</code> and <code>continue</code> in a <code>while</code> loop

count = 0
while count < 10:
    count += 1
    if count == 3:
        continue  # skip printing 3
    if count == 8:
        break     # stop the loop when count is 8
    print(count)
Note: Here, 3 is skipped due to <code>continue</code>, and the loop stops when count reaches 8 due to <code>break</code>.

<hr>

## Quiz on Loops

Write a <code>for</code> loop that prints out all the elements between <b>-5</b> and <b>5</b> using the range function.

# Write your code below and press Shift+Enter to execute
for i in range(-5,6):
    print(i)

<details><summary>Click here for the solution</summary>

```python
for i in range(-5, 6):
    print(i)
    
```

</details>

<hr>

Print the elements of the following list: <code>Genres=\[ 'rock', 'R\&B', 'Soundtrack', 'R\&B', 'soul', 'pop']</code>.
Make sure you follow Python conventions.

# Write your code below and press Shift+Enter to execute
Genres=[ 'rock', 'R&B', 'Soundtrack', 'R&B', 'soul', 'pop']

for Genre in Genres:
    print(Genre)
<details><summary>Click here for the solution</summary>

```python
Genres = ['rock', 'R&B', 'Soundtrack', 'R&B', 'soul', 'pop']
for Genre in Genres:
    print(Genre)
    
```

</details>

<hr>

Write a for loop that prints out the following list: <code>squares=\['red', 'yellow', 'green', 'purple', 'blue']</code>

# Write your code below and press Shift+Enter to execute

<details><summary>Click here for the solution</summary>

```python
squares=['red', 'yellow', 'green', 'purple', 'blue']
for square in squares:
    print(square)
    
```

</details>

<hr>

Write a while loop to display the values of the Rating of an album playlist stored in the<code>PlayListRatings</code> list. If the score is less than 6, exit the loop. The list <code>PlayListRatings</code> is given by: <code>PlayListRatings = \[10, 9.5, 10, 8, 7.5, 5, 10, 10]</code>

# Write your code below and press Shift+Enter to execute

<details><summary>Click here for the solution</summary>

```python
PlayListRatings = [10, 9.5, 10, 8, 7.5, 5, 10, 10]
i = 0
Rating = PlayListRatings[0]
while(i < len(PlayListRatings) and Rating >= 6):
    print(Rating)
    i = i + 1 # This prints the value 10 only once 
    Rating = PlayListRatings[i]
    i = i + 1 #Try uncommenting the line and comment the previous i = i + 1, and see the difference, 10 value will get printed twice because when the loop starts it will print Rating and then with PlayListRatings[0], it will again assign the value 10 to Ratings. 
    
```

</details>

<hr>

Write a while loop to copy the strings <code>'orange'</code> of the list <code>squares</code> to the list <code>new_squares</code>. Stop and exit the loop if the value on the list is not <code>'orange'</code>:

# Write your code below and press Shift+Enter to execute

squares = ['orange', 'orange', 'purple', 'blue ', 'orange']
new_squares = []

<details><summary>Click here for the solution</summary>

```python
squares = ['orange', 'orange', 'purple', 'blue ', 'orange']
new_squares = []
i = 0
while(i < len(squares) and squares[i] == 'orange'):
    new_squares.append(squares[i])
    i = i + 1
print (new_squares)
    
```

</details>

<hr>

Write a Python program using a for loop that prints numbers from 1 to 15 but:
- Skips multiples of 3
- Stops the loop if the number is greater than 12

# Write your code below and press Shift+Enter to execute
for i in range(1, 16):
    if i % 3 == 0:
        continue  # skip multiples of 3
    if i > 12:
        break     # stop if number > 12
    print(i)
        
<details><summary>Click here for the solution</summary>

```python
for i in range(1, 16):
    if i % 3 == 0:
        continue  # skip multiples of 3
    if i > 12:
        break     # stop if number > 12
    print(i)
        
```

</details>