<a id="dic"></a>
## Dictionaries

<a id="content"></a>
## What are Dictionaries?

A dictionary consists of keys and values. It is helpful to compare a dictionary to a list. Instead of being indexed numerically like a list, dictionaries have keys. These keys are the keys that are used to access values within a dictionary.   


The best example of a dictionary can be accessing person's detais using the **social security number**.   
Here the social security number which is a unique number will be the **key** and the details of the people will be the **values** associated with it.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/54cVKVMZaWEw7wSCDL8NjQ/DictList1.png" width="650">

### Create a Dictionary and access the elements

An example of a Dictionary <code>Dict</code>:
Here we are creating a dictionary named **Dict** with he following details

* Keys are **key1, key2, key3, key4, key5, (0,1)**.
* Values are {1,2,[3,3,3],(4,4,4),5,6} corresponding to the keys

# Create the dictionary

Dict = {"key1": 1, "key2": "2", "key3": [3, 3, 3], "key4": (4, 4, 4), ('key5'): 5, (0, 1): 6}
Dict
The keys can be strings:

# Access to the value by the key

Dict["key1"]
Keys can also be any immutable object such as a tuple:

# Access to the value by the key

Dict[(0, 1)]
Each key is separated from its value by a colon "<code>:</code>".  Commas separate the items, and the whole dictionary is enclosed in curly braces. An empty dictionary without any items is written with just two curly braces, like this  "<code>{}</code>".

# Create a sample dictionary

release_year_dict = {"Thriller": "1982", "Back in Black": "1980", \
                    "The Dark Side of the Moon": "1973", "The Bodyguard": "1992", \
                    "Bat Out of Hell": "1977", "Their Greatest Hits (1971-1975)": "1976", \
                    "Saturday Night Fever": "1977", "Rumours": "1977"}
release_year_dict
In summary, like a list, a dictionary holds a sequence of elements. Each element is represented by a key and its corresponding value. Dictionaries are created with two curly braces containing keys and values separated by a colon. For every key, there can only be one single value, however,  multiple keys can hold the same value. Keys can only be strings, numbers, or tuples, but values can be any data type.

It is helpful to visualize the dictionary as a table, as in the following image. The first column represents the keys, the second column represents the values.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%202/images/DictsStructure.png" width="650">

<a id="keys"></a>
## Keys

You can retrieve the values based on the names:

# Get value by keys

release_year_dict['Thriller'] 
This corresponds to:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%202/images/DictsKeyOne.png" width="500">

Similarly for <b>The Bodyguard</b>

# Get value by key

release_year_dict['The Bodyguard'] 
<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/Module%202/images/DictsKeyTwo.png" width="500">

Now let us retrieve the keys of the dictionary using the method <code>keys()</code>:

# Get all the keys in dictionary

release_year_dict.keys() 
You can retrieve the values using the method  <code>values()</code>:

# Get all the values in dictionary

release_year_dict.values() 
We can add an entry:

# Append value with key into dictionary

release_year_dict['Graduation'] = '2007'
release_year_dict
We can delete an entry:

# Delete entries by key

del(release_year_dict['Thriller'])
del(release_year_dict['Graduation'])
release_year_dict
We can verify if an element is in the dictionary:

# Verify the key is in the dictionary

'The Bodyguard' in release_year_dict
<hr>

<a id="quiz"></a>
## Quiz on Dictionaries

<b>You will need this dictionary for the next two questions:</b>

# Question sample dictionary

soundtrack_dic = {"The Bodyguard":"1992", "Saturday Night Fever":"1977"}
soundtrack_dic 
a) In the dictionary <code>soundtrack_dic</code> what are the keys ?

# Write your code below and press Shift+Enter to execute
soundtrack_dic.keys()
<details><summary>Click here for the solution</summary>

```python
soundtrack_dic.keys() # The Keys "The Bodyguard" and "Saturday Night Fever" 

```

</details>

b) In the dictionary <code>soundtrack_dic</code> what are the values ?

# Write your code below and press Shift+Enter to execute
soundtrack_dic.values()
<details><summary>Click here for the solution</summary>

```python
soundtrack_dic.values() # The values are "1992" and "1977"

```

</details>

<hr>

<b>You will need this dictionary for the following questions:</b>

The Albums <b>Back in Black</b>, <b>The Bodyguard</b> and <b>Thriller</b> have the following music recording sales in millions 50, 50 and 65 respectively:

a) Create a dictionary <code>album_sales_dict</code> where the keys are the album name and the sales in millions are the values.

# Write your code below and press Shift+Enter to execute
album_sales_dict = {"The Bodyguard":50, "Back in Black":50, "Thriller":65}
<details><summary>Click here for the solution</summary>

```python
album_sales_dict = {"The Bodyguard":50, "Back in Black":50, "Thriller":65}

```

</details>

b) Use the dictionary to find the total sales of <b>Thriller</b>:

# Write your code below and press Shift+Enter to execute
album_sales_dict["Thriller"]
<details><summary>Click here for the solution</summary>

```python
album_sales_dict["Thriller"]

```

</details>

c) Find the names of the albums from the dictionary using the method <code>keys()</code>:

# Write your code below and press Shift+Enter to execute
album_sales_dict.keys()
<details><summary>Click here for the solution</summary>

```python
album_sales_dict.keys()

```

</details>

d) Find the values of the recording sales from the dictionary using the method <code>values</code>:

# Write your code below and press Shift+Enter to execute
album_sales_dict.values()
<details><summary>Click here for the solution</summary>

```python
album_sales_dict.values()

```

</details>

<a id="Scenario"></a>
## Scenario:Inventory Store
    

The inventory store scenario project utilizes a dictionary-based approach to develop a robust system for managing and tracking inventory in a retail store.
<br>
**Note:- You will be working with two product details.**

## Task-1 Create an empty dictionary 


First you need to create an empty dictionary, where you will be storing the product details.

#Type your code here
inventory ={}
<details> <summary>Click here for the solution</summary>

```python

inventory ={}

```

</details>

## Task-2 Store the first product details in variable
* Product Name= Mobile phone
* Product Quantity= 5
* Product price= 20000
* Product Release Year= 2020

#type your code here
ProductNo1 = "Mobile Phone"
ProductNo1_quantity = 5
ProductNo1_price = 20000
ProductNo1_releaseYear= 2020
<details> <summary>Click here for the solution</summary>

```python
ProductNo1 = "Mobile Phone"
ProductNo1_quantity = 5
ProductNo1_price = 20000
ProductNo1_releaseYear= 2020
```

</details>

## Task-3 Add the details in inventory

#Type your code here
inventory["ProductNo1"]= ProductNo1
inventory["ProductNo1_quantity"]= ProductNo1_quantity
inventory["ProductNo1_price"]= ProductNo1_price
inventory["ProductNo1_releaseYear"]=ProductNo1_releaseYear
<details> <summary>Click here for the solution</summary>

```python

inventory["ProductNo1"]= ProductNo1
inventory["ProductNo1_quantity"]= ProductNo1_quantity
inventory["ProductNo1_price"]= ProductNo1_price
inventory["ProductNo1_releaseYear"]=ProductNo1_releaseYear

```

</details>

## Task-4 Store the second product details in a variable.
* Product Name= "Laptop"
* Product Quantity= 10
* Product price = 50000
* Product Release Year= 2023

#type your code here
ProductNo2 = "Laptop"
ProductNo2_quantity = 10
ProductNo2_price = 50000
ProductNo2_releaseYear= 2023
<details> <summary>Click here for the solution</summary>

```python

ProductNo2 = "Laptop"
ProductNo2_quantity = 10
ProductNo2_price = 50000
ProductNo2_releaseYear= 2023

```

</details>

## Task-5 Add the item detail into the inventory.

#type your code here
inventory["ProductNo2"]= ProductNo2
inventory["ProductNo2_quantity"]= ProductNo2_quantity
inventory["ProductNo2_price"]= ProductNo2_price
inventory["ProductNo2_releaseYear"]=ProductNo2_releaseYear
<details> <summary>Click here for the solution</summary>

```python

inventory["ProductNo2"]= ProductNo2
inventory["ProductNo2_quantity"]= ProductNo2_quantity
inventory["ProductNo2_price"]= ProductNo2_price
inventory["ProductNo2_releaseYear"]=ProductNo2_releaseYear

```

</details>

## Task-6 Display the Products present in the inventory

Use print statement for displaying the products


print(inventory)#type your code here
<details> <summary>Click here for the solution</summary>

```python

print(inventory)

```

</details>

## Task-7 Check if `ProductNo1_releaseYear` and `ProductNo2_releaseYear` is in the inventory

#Type your code here
print("ProductNo1_releaseYear" in inventory)
print("ProductNo2_releaseYear" in inventory)
<details> <summary>Click here for the solution</summary>

```python

print("ProductNo1_releaseYear" in inventory)
print("ProductNo2_releaseYear" in inventory)

```

</details>

**As in inventory `Release year` is not required, let's delete it.**

## Task-8 Delete release year of both the products from the inventory

#Type your code here

<details> <summary>Click here for the solution</summary>

```python

del(inventory["ProductNo1_releaseYear"])
del(inventory["ProductNo2_releaseYear"])

```

</details>