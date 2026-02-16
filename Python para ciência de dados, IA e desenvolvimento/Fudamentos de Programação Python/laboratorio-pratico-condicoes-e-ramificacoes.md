## Condition Statements

### Comparison Operators

Comparison operations compare some value or operand and based on a condition, produce a Boolean. When comparing two values you can use these operators:

<ul>
    <li>equal: <b>==</b></li>
    <li>not equal: <b>!=</b></li>
    <li>greater than: <b>></b></li>
    <li>less than: <b>&lt;</b></li>
    <li>greater than or equal to: <b>>=</b></li>
    <li>less than or equal to: <b>&lt;=</b></li>
</ul>

Let's assign <code> a </code> a value of 5. Use the equality operator denoted with two equal <b>==</b> signs to determine if two values are equal. The case below compares the variable <code>a</code> with 6.

# Condition Equal

a = 5
a == 6
The result is <b>False</b>, as 5 does not equal to 6.

Consider the following equality comparison operator: <code>i > 5</code>. If the value of the left operand, in this case the variable <b>i</b>, is greater than the value of the right operand, in this case 5, then the statement is <b>True</b>. Otherwise, the statement is <b>False</b>.  If <b>i</b> is equal to 6, because 6 is larger than 5, the output is <b>True</b>.

# Greater than Sign

i = 6
i > 5
Set <code>i = 2</code>. The statement is False as 2 is not greater than 5:

# Greater than Sign

i = 2
i > 5
Let's display some values for <code>i</code> in the figure. Set the values greater than 5 in green and the rest in red. The green region represents where the condition is **True**, the red where the statement is **False**. If the value of <code>i</code> is 2, we get **False** as the 2 falls in the red region. Similarly, if the value for <code>i</code> is 6 we get a **True** as the condition falls in the green region.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/CondsGreater.gif" width="650">

The inequality test uses an exclamation mark preceding the equal sign, if two operands are not equal then the condition becomes **True**.  For example, the following condition will produce **True** as long as the value of <code>i</code> is not equal to 6:

# Inequality Sign

i = 2
i != 6
When <code>i</code> equals 6 the inequality expression produces <b>False</b>.

# Inequality Sign

i = 6
i != 6
See the number line below. When the condition is **True**, the corresponding numbers are marked in green and for where the condition is **False** the corresponding number is marked in red.  If we set <code>i</code> equal to 2 the operator is true, since 2 is in the green region. If we set <code>i</code> equal to 6, we get a **False**, since the condition falls in the red region.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/CondsIneq.gif" width="650">

We can apply the same methods on strings. For example, we can use an equality operator on two different strings. As the strings are not equal, we get a **False**.

# Use Equality sign to compare the strings

"ACDC" == "The Bodyguard"
If we use the inequality operator, the output is going to be **True** as the strings are not equal.

# Use Inequality sign to compare the strings

"ACDC" != "The Bodyguard"
The inequality operation is also used to compare the letters/words/symbols according to the ASCII value of letters. The decimal value shown in the following table represents the order of the character:

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-7geq{background-color:#ffffc7;text-align:center;vertical-align:top}
.tg .tg-1cln{background-color:#ffcc67;font-size:100%;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-xozw{background-color:#ffcc67;font-weight:bold;text-align:center;vertical-align:top}
</style>

<table class="tg">
<thead>
  <tr>
    <th class="tg-1cln">Char.</th>
    <th class="tg-xozw">ASCII</th>
    <th class="tg-xozw">Char.</th>
    <th class="tg-xozw">ASCII</th>
    <th class="tg-xozw">Char.</th>
    <th class="tg-xozw">ASCII</th>
    <th class="tg-xozw">Char.</th>
    <th class="tg-xozw">ASCII</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7geq">A</td>
    <td class="tg-baqh">65</td>
    <td class="tg-7geq">N</td>
    <td class="tg-baqh">78</td>
    <td class="tg-7geq">a</td>
    <td class="tg-baqh">97</td>
    <td class="tg-7geq">n</td>
    <td class="tg-baqh">110</td>
  </tr>
  <tr>
    <td class="tg-7geq">B</td>
    <td class="tg-baqh">66</td>
    <td class="tg-7geq">O</td>
    <td class="tg-baqh">79</td>
    <td class="tg-7geq">b</td>
    <td class="tg-baqh">98</td>
    <td class="tg-7geq">o</td>
    <td class="tg-baqh">111</td>
  </tr>
  <tr>
    <td class="tg-7geq">C</td>
    <td class="tg-baqh">67</td>
    <td class="tg-7geq">P</td>
    <td class="tg-baqh">80</td>
    <td class="tg-7geq">c</td>
    <td class="tg-baqh">99</td>
    <td class="tg-7geq">p</td>
    <td class="tg-baqh">112</td>
  </tr>
  <tr>
    <td class="tg-7geq">D</td>
    <td class="tg-baqh">68</td>
    <td class="tg-7geq">Q</td>
    <td class="tg-baqh">81</td>
    <td class="tg-7geq">d</td>
    <td class="tg-baqh">100</td>
    <td class="tg-7geq">q</td>
    <td class="tg-baqh">113</td>
  </tr>
  <tr>
    <td class="tg-7geq">E</td>
    <td class="tg-baqh">69</td>
    <td class="tg-7geq">R</td>
    <td class="tg-baqh">82</td>
    <td class="tg-7geq">e</td>
    <td class="tg-baqh">101</td>
    <td class="tg-7geq">r</td>
    <td class="tg-baqh">114</td>
  </tr>
  <tr>
    <td class="tg-7geq">F</td>
    <td class="tg-baqh">70</td>
    <td class="tg-7geq">S</td>
    <td class="tg-baqh">83</td>
    <td class="tg-7geq">f</td>
    <td class="tg-baqh">102</td>
    <td class="tg-7geq">s</td>
    <td class="tg-baqh">115</td>
  </tr>
  <tr>
    <td class="tg-7geq">G</td>
    <td class="tg-baqh">71</td>
    <td class="tg-7geq">T</td>
    <td class="tg-baqh">84</td>
    <td class="tg-7geq">g</td>
    <td class="tg-baqh">103</td>
    <td class="tg-7geq">t</td>
    <td class="tg-baqh">116</td>
  </tr>
  <tr>
    <td class="tg-7geq">H</td>
    <td class="tg-baqh">72</td>
    <td class="tg-7geq">U</td>
    <td class="tg-baqh">85</td>
    <td class="tg-7geq">h</td>
    <td class="tg-baqh">104</td>
    <td class="tg-7geq">u</td>
    <td class="tg-baqh">117</td>
  </tr>
  <tr>
    <td class="tg-7geq">I</td>
    <td class="tg-baqh">73</td>
    <td class="tg-7geq">V</td>
    <td class="tg-baqh">86</td>
    <td class="tg-7geq">i</td>
    <td class="tg-baqh">105</td>
    <td class="tg-7geq">v</td>
    <td class="tg-baqh">118</td>
  </tr>
  <tr>
    <td class="tg-7geq">J</td>
    <td class="tg-baqh">74</td>
    <td class="tg-7geq">W</td>
    <td class="tg-baqh">87</td>
    <td class="tg-7geq">j</td>
    <td class="tg-baqh">106</td>
    <td class="tg-7geq">w</td>
    <td class="tg-baqh">119</td>
  </tr>
  <tr>
    <td class="tg-7geq">K</td>
    <td class="tg-baqh">75</td>
    <td class="tg-7geq">X</td>
    <td class="tg-baqh">88</td>
    <td class="tg-7geq">k</td>
    <td class="tg-baqh">107</td>
    <td class="tg-7geq">x</td>
    <td class="tg-baqh">120</td>
  </tr>
  <tr>
    <td class="tg-7geq">L</td>
    <td class="tg-baqh">76</td>
    <td class="tg-7geq">Y</td>
    <td class="tg-baqh">89</td>
    <td class="tg-7geq">l</td>
    <td class="tg-baqh">108</td>
    <td class="tg-7geq">y</td>
    <td class="tg-baqh">121</td>
  </tr>
  <tr>
    <td class="tg-7geq">M</td>
    <td class="tg-baqh">77</td>
    <td class="tg-7geq">Z</td>
    <td class="tg-baqh">90</td>
    <td class="tg-7geq">m</td>
    <td class="tg-baqh">109</td>
    <td class="tg-7geq">z</td>
    <td class="tg-baqh">122</td>
  </tr>
</tbody>
</table>

For example, the ASCII code for <b>!</b> is 33, while the ASCII code for <b>+</b> is 43. Therefore <b>+</b> is larger than <b>!</b> as 43 is greater than 33.

Similarly, from the table above we see that the value for <b>A</b> is 65, and the value for <b>B</b> is 66, therefore:

# Compare characters

'B' > 'A'
When there are multiple letters, the first letter takes precedence in ordering:

# Compare characters

'BA' > 'AB'
<b>Note</b>: Upper Case Letters have different ASCII code than Lower Case Letters, which means the comparison between the letters in Python is case-sensitive.

### Branching

Branching allows us to run different statements for different inputs. It is helpful to think of an **if statement** as a locked room, if the statement is **True** we can enter the room and your program will run some predefined tasks, but if the statement is **False** the program will ignore the task.

For example, consider the blue rectangle representing an ACDC concert. If the individual is older than 18, they can enter the ACDC concert. If they are 18 or younger, they cannot enter the concert.

We can use the condition statements learned before as the conditions that need to be checked in the **if statement**. The syntax is as simple as <code> if <i>condition statement</i> :</code>, which contains a word <code>if</code>, any condition statement, and a colon at the end. Start your tasks which need to be executed under this condition in a new line with an indent. The lines of code after the colon and with an indent will only be executed when the **if statement** is **True**. The tasks will end when the line of code does not contain the indent.

In the case below, the code <code>print(“you can enter”)</code> is executed only if the variable <code>age</code> is greater than 18 is a True case because this line of code has the indent. However, the execution of <code>print(“move on”)</code> will not be influenced by the if statement.

# If statement example

age = 19
#age = 18

#expression that can be true or false
if age > 18:
    
    #within an indent, we have the expression that is run if the condition is true
    print("you can enter" )

#The statements after the if statement will run regardless if the condition is true or false 
print("move on")
<i>Try uncommenting the age variable</i>

It is helpful to use the following diagram to illustrate the process. On the left side, we see what happens when the condition is <b>True</b>.  The person enters the ACDC concert representing the code in the indent being executed; they then move on. On the right side, we see what happens when the condition is <b>False</b>; the person is not granted access, and the person moves on. In this case, the segment of code in the indent does not run, but the rest of the statements are run.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/CondsIf.gif" width="650">

The <code>else</code> statement runs a block of code if none of the conditions are **True** before this <code>else</code> statement. Let's use the ACDC concert analogy again. If the user is 17 they cannot go to the ACDC concert,  but they can go to the Meatloaf concert.
The syntax of the <code>else</code> statement is similar as the syntax of the <code>if</code> statement, as <code>else :</code>. Notice that, there is no condition statement for <code>else</code>.
Try changing the values of <code>age</code> to see what happens:

# Else statement example

age = 18
# age = 19

if age > 18:
    print("you can enter" )
else:
    print("go see Meat Loaf" )
    
print("move on")
The process is demonstrated below, where each of the possibilities is illustrated on each side of the image. On the left is the case where the age is 17, we set the variable age to 17, and this corresponds to the individual attending the Meatloaf concert. The right portion shows what happens when the individual is over 18, in this case 19, and the individual is granted access to the concert.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/CondsElse.gif" width="650">

The <code>elif</code> statement, short for else if, allows us to check additional conditions if the condition statements before it are <b>False</b>. If the condition for the <code>elif</code> statement is <b>True</b>, the alternate expressions will be run. Consider the concert example, where if the individual is 18 they will go to the Pink Floyd concert instead of attending the ACDC or Meat-loaf concert. A person that is 18 years of age enters the area, and as they are not older than 18 they can not see ACDC, but since they are 18 years of age, they attend  Pink Floyd. After seeing Pink Floyd, they move on. The syntax of the <code>elif</code> statement is similar in that we merely change the <code>if</code> in the <code>if</code> statement to <code>elif</code>.

# Elif statment example

age = 18

if age > 18:
    print("you can enter" )
elif age == 18:
    print("go see Pink Floyd")
else:
    print("go see Meat Loaf" )
    
print("move on")
The three combinations are shown in the figure below.  The left-most region shows what happens when the individual is less than 18 years of age. The central component shows when the individual is exactly 18. The rightmost shows when the individual is over 18.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/CondsElif.gif" width="650">

Look at the following code:

# Condition statement example

album_year = 1983
album_year = 1970

if album_year > 1980:
    print("Album year is greater than 1980")
    
print('do something..')
Feel free to change <code>album_year</code> value to other values -- you'll see that the result changes!

Notice that the code in the above <b>indented</b> block will only be executed if the results are <b>True</b>.

As before, we can add an <code>else</code> block to the <code>if</code> block. The code in the <code>else</code> block will only be executed if the result is <b>False</b>.

<b>Syntax:</b>

if (condition):
\# do something
else:
\# do something else

If the condition in the <code>if</code> statement is <b>False</b>, the statement after the <code>else</code> block will execute. This is demonstrated in the figure:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/CondsLogicMap.png" width="650">

# Condition statement example

album_year = 1983
#album_year = 1970

if album_year > 1980:
    print("Album year is greater than 1980")
else:
    print("less than 1980")

print('do something..')
Feel free to change the <code>album_year</code> value to other values -- you'll see that the result changes based on it!

### Logical operators

Sometimes you want to check more than one condition at once. For example, you might want to check if one condition and another condition are both **True**. Logical operators allow you to combine or modify conditions.

<ul>
    <li><code>and</code></li>
    <li><code>or</code></li>
    <li><code>not</code></li>
</ul>

These operators are summarized for two variables using the following truth tables:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/CondsTable.png" width="650">

The <code>and</code> statement is only **True** when both conditions are true. The <code>or</code> statement is True if one condition, or both are **True**. The <code>not</code> statement outputs the opposite truth value.

Let's see how to determine if an album was released after 1979 (1979 is not included) and before 1990 (1990 is not included). The time periods between 1980 and 1989 satisfy this condition. This is demonstrated in the figure below. The green on lines <strong>a</strong> and <strong>b</strong> represents periods where the statement is **True**. The green on line <strong>c</strong> represents where both conditions are **True**, this corresponds to where the green regions overlap.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/CondsEgOne.png" width="650">

The block of code to perform this check is given by:

# Condition statement example

album_year = 1980

if(album_year > 1979) and (album_year < 1990):
    print ("Album year was in between 1980 and 1989")
    
print("")
print("Do Stuff..")
To determine if an album was released before 1980 (1979 and earlier) or after 1989 (1990 and onward ), an or statement can be used. Periods before 1980 (1979 and earlier) or after 1989 (1990 and onward) satisfy this condition. This is demonstrated in the following figure, the color green in <strong>a</strong> and <strong>b</strong> represents periods where the statement is true. The color green in **c** represents where at least one of the conditions
are true.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%203/images/CondsEgTwo.png" width="650">

The block of code to perform this check is given by:

# Condition statement example

album_year = 1990

if(album_year < 1980) or (album_year > 1989):
    print ("Album was not made in the 1980's")
else:
    print("The Album was made in the 1980's ")
The <code>not</code> statement checks if the statement is false:

# Condition statement example

album_year = 1983

if not (album_year == 1984):
    print ("Album year is not 1984")
<hr>

## Quiz on Conditions

Analyze a dataset containing information about renowned athletes, including their names, sports, and notable achievements, to apply conditional logic and filtering techniques.

<table border="1">
  <tr>
    <th>Player Name</th>
    <th>Sport</th>
    <th>Achievements</th>
  </tr>
  <tr>
    <td>Serena Williams</td>
    <td>Tennis</td>
    <td>23 Grand Slams</td>
  </tr>
  <tr>
    <td>Lionel Messi</td>
    <td>Soccer</td>
    <td>7 Ballon d'Ors</td>
  </tr>
  <tr>
    <td>Michael Phelps</td>
    <td>Swimming</td>
    <td>23 Gold Medals</td>
  </tr>
  <tr>
    <td>Usain Bolt</td>
    <td>Athletics</td>
    <td>8 Gold Medals</td>
  </tr>
  <tr>
    <td>Roger Federer</td>
    <td>Tennis</td>
    <td>20 Grand Slams</td>
  </tr>
  <tr>
    <td>Cristiano Ronaldo</td>
    <td>Soccer</td>
    <td>5 Ballon d'Ors</td>
  </tr>
</table>

Write a Python program to check if a player <b>Lionel Messi</b> has more than 10 achievements. If the condition is true, print the player's name, sport, and achievements else print does not have more than 10 achievements.

# Write your code below and press Shift+Enter to execute
player_name = "Lionel Messi"
sport = "Soccer"
achievements = 7

if achievements > 10:
    print(f"{player_name} plays {sport} and has {achievements} achievements.")
else:
    print(f"{player_name} does not have more than 10 achievements.")
<details><summary>Click here for the solution</summary>
    
```python
player_name = "Lionel Messi"
sport = "Soccer"
achievements = 7

if achievements > 10:
    print(f"{player_name} plays {sport} and has {achievements} achievements.")
else:
    print(f"{player_name} does not have more than 10 achievements.")
```
</details>

<hr>

Write a Python program to check if a player belongs to the sport Tennis or has exactly 20 achievements. If the condition is true, print a success message.

# Write your code below and press Shift+Enter to execute

<details><summary>Click here for the solution</summary>

```python
player_name = "Roger Federer"
sport = "Tennis"
achievements = 20

if sport == "Tennis" or achievements == 20:
    print(f"{player_name} meets the criteria! They play {sport} and have {achievements} achievements.")
else:
    print(f"{player_name} does not meet the criteria.")
```

</details>

<hr>

Write a Python program to check if a player has less than 10 achievements and does not play Soccer. Print their details if they meet the criteria.

# Write your code below and press Shift+Enter to execute

<details><summary>Click here for the solution</summary>

```python
player_name = "Usain Bolt"
sport = "Athletics"
achievements = 8

if achievements < 10 and sport != "Soccer":
    print(f"{player_name} plays {sport} and has only {achievements} achievements.")
else:
    print(f"{player_name} does not meet the criteria.")
```

</details>