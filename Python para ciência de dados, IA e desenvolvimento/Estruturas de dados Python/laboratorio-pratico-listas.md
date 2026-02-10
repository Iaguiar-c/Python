<a id="dataset"></a>
## About the Dataset

Imagine you received album recommendations from your friends and compiled all of the recommandations into a table, with specific information about each album.

The table has one row for each movie and several columns:

*   **Artist** - Name of the artist
*   **Album** - Name of the album
*   **Released_year** - Year the album was released
*   **Length_min_sec** - Length of the album (hours,minutes,seconds)
*   **Genre** - Genre of the album
*   **Music_recording_sales_millions** - Music recording sales (millions in USD) on [SONG://DATABASE](http://www.song-database.com/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkPY0101ENSkillsNetwork19487395-2021-01-01)
*   **Claimed_sales_millions** - Album's claimed sales (millions in USD) on [SONG://DATABASE](http://www.song-database.com/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkPY0101ENSkillsNetwork19487395-2021-01-01)
*   **Released** - Date on which the album was released
*   **Soundtrack** - Indicates if the album is the movie soundtrack (Y) or (N)
*   **Rating_of_friends** - Indicates the rating from your friends from 1 to 10

<br>
<br>

The Dataset can be seen below:

<font size="1">
<table font-size:xx-small>
  <tr>
    <th>Artist</th>
    <th>Album</th> 
    <th>Released</th>
    <th>Length</th>
    <th>Genre</th> 
    <th>Music recording sales (millions)</th>
    <th>Claimed sales (millions)</th>
    <th>Released</th>
    <th>Soundtrack</th>
    <th>Rating (friends)</th>
  </tr>
  <tr>
    <td>Michael Jackson</td>
    <td>Thriller</td> 
    <td>1982</td>
    <td>00:42:19</td>
    <td>Pop, rock, R&B</td>
    <td>46</td>
    <td>65</td>
    <td>30-Nov-82</td>
    <td></td>
    <td>10.0</td>
  </tr>
  <tr>
    <td>AC/DC</td>
    <td>Back in Black</td> 
    <td>1980</td>
    <td>00:42:11</td>
    <td>Hard rock</td>
    <td>26.1</td>
    <td>50</td>
    <td>25-Jul-80</td>
    <td></td>
    <td>8.5</td>
  </tr>
    <tr>
    <td>Pink Floyd</td>
    <td>The Dark Side of the Moon</td> 
    <td>1973</td>
    <td>00:42:49</td>
    <td>Progressive rock</td>
    <td>24.2</td>
    <td>45</td>
    <td>01-Mar-73</td>
    <td></td>
    <td>9.5</td>
  </tr>
    <tr>
    <td>Whitney Houston</td>
    <td>The Bodyguard</td> 
    <td>1992</td>
    <td>00:57:44</td>
    <td>Soundtrack/R&B, soul, pop</td>
    <td>26.1</td>
    <td>50</td>
    <td>25-Jul-80</td>
    <td>Y</td>
    <td>7.0</td>
  </tr>
    <tr>
    <td>Meat Loaf</td>
    <td>Bat Out of Hell</td> 
    <td>1977</td>
    <td>00:46:33</td>
    <td>Hard rock, progressive rock</td>
    <td>20.6</td>
    <td>43</td>
    <td>21-Oct-77</td>
    <td></td>
    <td>7.0</td>
  </tr>
    <tr>
    <td>Eagles</td>
    <td>Their Greatest Hits (1971-1975)</td> 
    <td>1976</td>
    <td>00:43:08</td>
    <td>Rock, soft rock, folk rock</td>
    <td>32.2</td>
    <td>42</td>
    <td>17-Feb-76</td>
    <td></td>
    <td>9.5</td>
  </tr>
    <tr>
    <td>Bee Gees</td>
    <td>Saturday Night Fever</td> 
    <td>1977</td>
    <td>1:15:54</td>
    <td>Disco</td>
    <td>20.6</td>
    <td>40</td>
    <td>15-Nov-77</td>
    <td>Y</td>
    <td>9.0</td>
  </tr>
    <tr>
    <td>Fleet wood Mac</td>
    <td> Rumours </td> 
    <td>1977</td>
    <td>00:40:01</td>
    <td>Soft rock</td>
    <td>27.9</td>
    <td>40</td>
    <td>04-Feb-77</td>
    <td></td>
    <td>9.5</td>
  </tr>
</table></font>

<hr>

<a id="list"></a>
## Lists


<a id="index"></a>
## Indexing

We are going to take a look at lists in Python. A list is a sequenced collection of different objects such as integers, strings, and even other lists as well. The address of each element within a list is called an <b>index</b>. An index is used to access and refer to items within a list.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%202/images/ListsIndex.png" width="1000">

To create a list, type the list within square brackets <b>\[ ]</b>, with your content inside the parenthesis and separated by commas. Let us try it!

# Create a list

L = ["The Bodyguard", 7.0, 1992]
L
We can use negative and regular indexing with a list:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/kkMiHZTtmXzY4BWInK5Azg/Slide1.PNG" width="1000">

# Print the elements on each index

print('the same element using negative and positive indexing:\n Postive:',L[0],
'\n Negative:' , L[-3]  )
print('the same element using negative and positive indexing:\n Postive:',L[1],
'\n Negative:' , L[-2]  )
print('the same element using negative and positive indexing:\n Postive:',L[2],
'\n Negative:' , L[-1]  )
<a id="content"></a>
## List Content

Lists can contain strings, floats, and integers. We can nest other lists, and we can also nest tuples and other data structures. The same indexing conventions apply for nesting:

# Sample List

["The Bodyguard", 7.0, 1992, [1, 2], ("A", 1)]
<a id="op"></a>
## List Operations

We can also perform slicing in lists. For example, if we want the last two elements, we use the following command:

# Sample List

L = ["The Bodyguard", 7.0,1992,"BG",1]
L
<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/KyRT0sxnEHkVDzA5XS6h0w/Slide2.PNG" width="1000">

# List slicing

L[3:5]
We can use the method <code>extend</code> to add new elements to the list:

# Use extend to add elements to list

L = [ "The Bodyguard", 7.0]
L.extend(['pop', 10])
L
Another similar method is <code>append</code>. If we apply <code>append</code> instead of <code>extend</code>, we add one element to the list:

# Use append to add elements to list

L = [ "The Bodyguard", 7.0]
L.append(['pop', 10])
L
Each time we apply a method, the list changes. If we apply <code>extend</code> we add two new elements to the list. The list <code>L</code> is then modified by adding two new elements:

# Use extend to add elements to list

L = [ "The Bodyguard", 7.0]
L.extend(['pop', 10])
L
If we append the list  <code>\['a','b']</code> we have one new element consisting of a nested list:

# Use append to add elements to list

L.append(['a','b'])
L
As lists are mutable, we can change them. For example, we can change the first element as follows:

# Change the element based on the index

A = ["disco", 10, 1.2]
print('Before change:', A)
A[0] = 'hard rock'
print('After change:', A)
We can also delete an element of a list using the <code>del</code> command:

# Delete the element based on the index

print('Before change:', A)
del(A[0])
print('After change:', A)
We can convert a string to a list using <code>split</code>.  For example, the method <code>split</code> translates every group of characters separated by a space into an element in a list:

# Split the string, default is by space

'hard rock'.split()
We can use the split function to separate strings on a specific character which we call a **delimiter**. We pass the character we would like to split on into the argument, which in this case is a comma.  The result is a list, and each element corresponds to a set of characters that have been separated by a comma:

# Split the string by comma

'A,B,C,D'.split(',')
<a id="co"></a>
## Copy and Clone List

When we set one variable <b>B</b> equal to <b>A</b>, both <b>A</b> and <b>B</b> are referencing the same list in memory:

# Copy (copy by reference) the list A

A = ["hard rock", 10, 1.2]
B = A
print('A:', A)
print('B:', B)
<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%202/images/ListsRef.png" width="1000" align="center">

Initially, the value of the first element in <b>B</b> is set as "hard rock". If we change the first element in <b>A</b> to <b>"banana"</b>, we get an unexpected side effect.  As <b>A</b> and <b>B</b> are referencing the same list, if we change list <b>A</b>, then list <b>B</b> also changes. If we check the first element of <b>B</b> we get "banana" instead of "hard rock":

# Examine the copy by reference

print('B[0]:', B[0])
A[0] = "banana"
print('B[0]:', B[0])
This is demonstrated in the following figure:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%202/images/ListsRefGif.gif" width="1000">

You can clone list **A** by using  the following syntax:

# Clone (clone by value) the list A

B = A[:]
B
Variable **B** references a new copy or clone of the original list. This is demonstrated in the following figure:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%202/images/ListsVal.gif" width="1000">

Now if you change <b>A</b>, <b>B</b> will not change:

print('B[0]:', B[0])
A[0] = "hard rock"
print('B[0]:', B[0])
<a id="quiz"></a>
## Quiz on List

Create a list <code>a_list</code>, with the following elements <code>1</code>, <code>hello</code>, <code>\[1,2,3]</code> and <code>True</code>.

# Write your code below and press Shift+Enter to execute
a_list = [1, 'hello', [1,2,3], True]
a_list

<details><summary>Click here for the solution</summary>

```python
a_list = [1, 'hello', [1, 2, 3] , True]
a_list

```

</details>

Find the value stored at index 1 of <code>a_list</code>.

# Write your code below and press Shift+Enter to execute
a_list[1]
<details><summary>Click here for the solution</summary>

```python
a_list[1]

```

</details>

Retrieve the elements stored at index 1, 2 and 3 of <code>a_list</code>.

# Write your code below and press Shift+Enter to execute
a_list[1:4]
<details><summary>Click here for the solution</summary>

```python
a_list[1:4]

```

</details>

Concatenate the following lists <code>A = \[1, 'a']</code> and <code>B = \[2, 1, 'd']</code>:

# Write your code below and press Shift+Enter to execute
A = [1,'a']
B = [2,1,'d']
A+B
<details><summary>Click here for the solution</summary>

```python
A = [1, 'a'] 
B = [2, 1, 'd']
A + B

```

</details>

<a id="Scenario"></a>
## Scenario : Shopping list 

# Task-1  Create an empty list
At first we need to create a empty list for storing the items to buy in Shopping list.

#Type your code here
Shopping_list = []
<details><summary>Click here for the solution</summary>

```python
Shopping_list=[]

```

</details>

# Task-2 Now store the number of items to the shopping_list
* Watch
* Laptop
* Shoes
* Pen
* Clothes


<br>


#Type your code here
Shopping_list = ["Watch", "Laptop", "Shoes", "Pen", "Clothes"]
<details><summary>Click here for the hint </summary>

```python
Hint:- Directly store every item as a different string in the list.

```

</details>

<details><summary>Click here for the solution</summary>

```python
Shopping_list=["Watch","Laptop","Shoes","Pen","Clothes"]

```

</details>

# Task-3 Add a new item to the shopping_list
Seems like I missed one item "Football" to add in the shopping list.
<br>

#Type your code here
Shopping_list.append("Football")
<details><summary>Click here for the hint </summary>

```python
Hint:- Use `Append()` method for adding "Football" to our shopping list

```

</details>

<details><summary>Click here for the solution</summary>

```python
Shopping_list.append("Football")

```

</details>

# Task-4 Print First item from the shopping_list
Let's check the first item that we need to buy.
<br>

#Type your code here
print(Shopping_list[0])
<details><summary>Click here for the hint </summary>

```python
Hint:- Use `indexing` for checking the first item.

```

</details>

<details><summary>Click here for the solution</summary>

```python
print(Shopping_list[0])

```

</details>

# Task-5 Print Last item from the shopping_list
Let's check the last time that we need to buy.
<br>

#Type your code here
print(Shopping_list[-1])
<details><summary>Click here for the hint </summary>

```python
Hint:- Use `indexing` for checking for last item.

```

</details>

<details><summary>Click here for the solution</summary>

```python
print(Shopping_list[-1])

```

</details>

# Task-6 Print the entire Shopping List

#Type your code here.
print(Shopping_list)
<details><summary>Click here for the solution</summary>

```python
print(Shopping_list)

```

</details>

# Task-7 Print the item that are important to buy from the Shopping List
Print "Laptop" and "shoes"

#Type your code here
print(Shopping_list[1:3])
<details><summary>Click here for the hint </summary>

```python
Hint:- Use `slicing` to print "Laptop" and "Shoes"

```

</details>

<details><summary>Click here for the solution</summary>

```python
print(Shopping_list[1:3])

```

</details>

# Task-8 Change the item from the shopping_list 
Instead of <u>"Pen"</u> I want to buy <u>"Notebook"</u>
let's change the item stored in the list.
<br>


#Type your code here
Shopping_list[3]
<details><summary>Click here for the hint </summary>

```python
Hint:- Locate the item you want to change using `index`, and Update the item with the new desired value using `string`.

```

</details>

<details><summary>Click here for the solution</summary>

```python
Shopping_list[3] = "Notebook"

```

</details>

# Task-9 Delete the item from the shopping_list that is not required
Let's delete items that are unimportant, such as; I don't want to buy <u>Clothes</u>, let's delete it.
<br>


#Type your code here
<details><summary>Click here for the hint </summary>

```python
Hint:- Use `del` method for deleting.

```

</details>

<details><summary>Click here for the solution</summary>

```python
del (Shopping_list[4])

```

</details>

# Task-10 Print the shopping list
We are ready with our shopping list.

# Type your code here
<details><summary>Click here for the solution</summary>

```python
print(Shopping_list)

```