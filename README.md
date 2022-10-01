# Python Guide #2
## List, Set, and String Operations ##

* `len()` , this method will return the sum of the total items in an object. on a string, this function will return the number of characters.
* `min()` and `max()`. this method are to find out what the minimum and maximum values are.
* `count()`, this method is to find out how many times an object appears in the list.
* `sort()`, this method sorts the list ascending by default and alse can be use dby specifying sorting criteria, such as key and reverse.
   - parameter `reverse` is used to choose sorting type like descending or ascending.
   - parameter `key` is used to specify the sorting criteria.
   
#### Concatenation ####
concatenation means joining strings together end-to-end to create a new string use the `+` operator.

![image](https://user-images.githubusercontent.com/91566708/193400969-0f2c4092-8ef0-49fe-8f47-f70f74137177.png)

#### Replication ####
replication is multiplication operator `*`. when used with one string and one integer, this operator `*` will reapating a single string however many times the given integer.

![image](https://user-images.githubusercontent.com/91566708/193401032-877a3024-27b7-4a43-a3ab-98f672709d7d.png)

#### Range ####
1. one parameter `range(n)`, is used to create a series of numbers starting from 0 to **n**.
2. two parameter `range(n,p)`, is used to create a series of numbers starting from **n** until before **p**.
3. three parameter `range(n,p,q)`, is used to create a series of numbers starting from **n**, until before **p**, with each element having a difference of **q**.

#### In and Not In #####
operators `in` and `not in`, to find out a value or object is in a list. This function will retrun a boolean value true or false.

#### Assign Values To Multiple Variables ####
In assigning values to multiple variables, conventionally, we can mark the variables with the values you want, one at a time. But, Python has a more practical way, which is that we can assign values to multiple variables at once from a list or tuple element without needing to mark them one by one.

![image](https://user-images.githubusercontent.com/91566708/193401318-c6b31406-7236-4cd7-9cfd-98621020dae9.png)

In an hewan2 list, there are 3 values in it. We want to define some different variable for each value in the list, so we can do this simultaneously by using a comma `,`.


## Operator, Operands, and Expressions

### Arithmetic Operator ###
* Addition `+` , math operation in which we add the numbers together to get their sum.
* Subtraction `-` , taking something away from a number.
* Multiplication `*` , to process of calculating the result when a number is taken times.
* Division `/` , to process of splitting a specific amount into equal parts.
* Modulus `%` , is the remainder after dividing one number by another.
* Exponentiation `**` , in math is defined as the operation used to represent repeated multiplication.
* Floor Division `//` , a normal division operation except that it returns the largest possible integer.

### Logical Operator ###
* Equal `==`

![image](https://user-images.githubusercontent.com/91566708/193291619-0f53d82c-7257-4500-a6d0-ef2f237dbf9a.png)

* Not equal `!=`

![image](https://user-images.githubusercontent.com/91566708/193291699-7083e9c0-78b9-4452-bb6d-2c28770c6573.png)

* Greater than `>`

![image](https://user-images.githubusercontent.com/91566708/193291470-15468497-9965-4791-920e-3f853b0ce397.png)

* Less than `<`

![image](https://user-images.githubusercontent.com/91566708/193291544-c6e12d2c-ba37-4b3d-8c36-4f94e60b9a1d.png)

* Greater than or equal to `>=`

![image](https://user-images.githubusercontent.com/91566708/193291780-7d968373-f47e-4702-9953-a98c1cac6a00.png)

* Less than or equal to `<=`

![image](https://user-images.githubusercontent.com/91566708/193291851-2b9127f2-b31f-4bf3-9512-65bc35499e6b.png)

### Boolean ###
* `and`, is used to combine conditional statemnets. Both conditions must be fullfilled.

![image](https://user-images.githubusercontent.com/91566708/193401534-14bfbbf4-994f-4442-a560-7fc270ac04c8.png)

* `or`, is used to check that there is at least on true. If just one side i strue the entire expression is true. Just one condition must be fullfilled.

![image](https://user-images.githubusercontent.com/91566708/193401549-e2eaf72c-3b28-43e7-af39-4cd0fa5c05b1.png)

### Python Assignment Operator ###
* `=` equal.
* `+=` add and assign.
* `-=` subtract and.
* `/=` divide and.
* `*=` multiply and.
* `%=` modulus and.
* `**=` exponent and.
* `//=` floor division.

##### example #####

```py
  x = 10   
  
  # add and assign
  x += 2 # x = 12
  
  # subtract and
  x -= 2 # x = 8
  
  # divide and
  x /= 2 # x = 5.0
  
  # multiply and
  x *= 2 # x = 20
  
  # exponent and
  x **= 2 # x = 1000
  
  # modulus and
  x %= 2 # x = 1
  
  # floor division
  x //= 2 # x = 3
```

### Precendence Operator ###
python will always evaluate the arithmetic operators first

![image](https://user-images.githubusercontent.com/91566708/193402094-d17ccc2d-df45-4cf2-8deb-ad81b58614d6.png)

## Conditional Expression ##

![image](https://user-images.githubusercontent.com/91566708/193402730-d293959a-d47a-4780-8c9f-f9108a3bc734.png)

1. `if`
only a statement is True will be executd, if it is false it will not. In python, the body of the if the indentation indicates statement, the body starts with an indentation and the first unindented line marks the end. The output is non-zero values as true, none and () are interpreted as false.

2. `else`
The if...else statement evaluates test expression and will execute the body of id only when the test condition is true. if it is false it will not. 

3. `elif`
If the condition for if is false, it checks the condition of the next elif block and so on. if it is false the body of else is executed. Only one block among the several `if`...`elif`...`else` block is executed according to the condition. In other words, we can say that elif is python way of sating "if the previous conditions were not true, then try this condition".

## Loops ##

### Types ###
* **for Loops**
For loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string). This is less like the for keyword in other programming languages, and works more like an iterator method as found in other object-orientated programming languages.

![image](https://user-images.githubusercontent.com/91566708/193402754-60878957-a963-439d-b810-670cf92aedda.png)

* **Nested Loops**
Nested loop is a loop inside a loop. The "inner loop" will be executed one time for each iteration of the "outer loop".

![image](https://user-images.githubusercontent.com/91566708/193402764-19a6c8c6-ea48-47a5-875f-d269fbe7f3d0.png)

* **While Loops**
The while statement creates a loop that executes a specified statement as long as the test condition evaluates to true. The condition is evaluated before executing the statement.

![image](https://user-images.githubusercontent.com/91566708/193402778-a14e4817-2bcf-4f0d-8d6a-26723ca40d6e.png)

### Loops Control State Statement ###

* **Break**, is used to terminate the loop.
* **continue**, is used when we want to skip a particular condition and continue the rest execution.
* **pass**, is used as a placeholder for future code. When it's executed, nothin happen, but you avoid getting an error.

## List Comprehension ##
list comprehension is a way to generate new lists based on pre-existing lists or iterables. To create list comprehension you can use this syntax.

![image](https://user-images.githubusercontent.com/91566708/193402617-20696bc8-5d5e-4975-877e-4867aa347d94.png)

underscore `_` including valid variable naming. In general `_` can be used as a throwaway variable (variable is not to imporntant).

## Types Of Error In Python Programming Language ##

### Based On Occurrence
* syntax error, occur when python can't understant what we mean.
* exceptions, ooccur while the  process is in progress are called exceptions and can be fatal if not handled.

