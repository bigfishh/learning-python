## Data Types and Variables

* No emphasis on declaring datatypes
* Three main data types 
    * Numbers 
    * Strings
    * Booleans 
* Variables can be used to give a name to data 
    * They are mutable -- can be updated and replaced 

### Numbers

* Python automatically converts integer to floating-point when you're doing calculations between an integer and a floating-point
* Three main types of numbers
    * Integer 
    * Floating Point Numbers 
    * Complex Numbers 
* Integer 
    * Made up of positive + negative whole numbers 
    * Depending on the value of the integer, it will take up different amount of memory
    * Ex: `0` -> 24 bytes, `1` -> 28 bytes 
* Floating Point Numbers 
    * Made up of positive + negative decimal numbers 
    * Useful for precise calculations of values 
    * Takes up 24 bytes of memory 
* Complex Numbers 
    * Numbers that are made up of real and an imaginary part. 
    * `complex(real, imaginary)` can be used to create complex numbers 
    * Takes in two parts: real number and imaginary number
    * For imaginary, it will attach a `j` behind the imaginary argument that's passed in
    * Takes up 32 bytes of memory 


### Booleans

* Bool 
* Has two values: `True` and `False`
* Useful to logic and data comparison 


### Strings
 
* Collections of chracters enclosed by `""` or `''`
* `len("will return the length of this string")`
* Indexing starts from zero 
* Each character can be accessed by enclosing the index with square brackets, `[]`
* Reverse indexing can be implemented by using a negative value, ex: `-1` refers to the last index of a string
* String slicing: 
    * Obtaining only a portion of the string
    * `string[start:end]`
        * The `start` is the index that you're starting from 
        * `end` is the index that you're ending at, not included. 
    * `string[start:end:step]`
        * Skipping characters,`step` 
        * Reverse slicing from the end to the front; the starting value is larger than the ending value and there must to be a negative value for the `step`
            * Ex: `string[20:2:-1]`
    * Partial slicing can happening if either the `start` or the `end` is left out 
        * If `start` is left out -- the slicing will start from the `0` index and stop at the `end` index
        * If `end` if left out -- the slicing will start  from the `start` index and end at the `n-1` index
* `in` keyword to check if a substring is included in another string 
    * ex: `"hi" in "hi panda"` return true

### Operators 

* in-fix notation 
    * the operator appears between the values that it's operated on 
    * aka binary operator 
* prefix notation 
    * appears before the value it is operated on
    * aka unary operator
* five main operator in Python 
    * arithmetic 
        * exponent `**`
        * modulo `%`
        * multiplication `*`
        * division `/`
        * floor division `//`
            * the result is floored to the nearest smallest integer 
            * aka integer division 
        * addition `+`
        * subtraction `-`
    * comparison 
        * `>`, `<`, `>=`, `<=`, `==`, `is` (equal to), `is not` (not equal to)
    * assignment 
        * `=`, `+=`, `-=`, `*=`, `/=`. `//=`, `**=`, `%=`, `|=` (OR), `&=` (AND), `^=` (^=), `>>=`, `<<=`
    * logical 
        * `and`, `or`, `not`
        * programming is made of combinations of `1`s and `0`s. 
            * `1`s represents `True`
            * `0`s represents `False`
    * bitwise 
        * `&` - Bitwise AND
        * `|` - Bitwise OR
        * `^` - Bitwise XOR
        * `~` - Bitwise NOT
        * `<<` - Shift Bit Left
        * `>>` - Shift Bitwise Right

### List 

* a collection of values enclosed in square brackets, `[]`

### Conditional Statements 

* control flow statement, allows for multiple endpoints depending on which condition is satisfied. 
*  `if` statement
    * indentation really matters in ruby, they indicate blocks, `inner` and `inter-related` blocks
```python
num == 300 

if (num == 20): 
    print("hello, I'm 20")

# nested if statements 
if (num > 20):
    if (num > 100): 
        if (num > 200):
            print("hello, I'm greater than 20")
```
* `if-else` statement
    * the `if` and the `else` are at the same indentation level
```python 
weather = "rainy"

if weather == "rainy":
    print("remember to bring an umbrella")
else:
    print("it's not raining today")

# conditonal statement -- same as above
output = "remember to bring an umbrella" \ 
    if weather == "rainy" else "it's not raining today"

print(output)
```
* `if-elif-else` statement
    * `elif` stand for else if 
    * `else` can be excluded from the statement 
    * `if`, `elif`, and `else` are on the same indentation level 
```python 

season = "Winter"

if season == "Winter":
    print("Let's build a snowman")

elif season == "Autumn":
    print("Let's go apple picking")

elif season == "Summer":
    print("Let's go to the beach")
    
elif season == "Spring":
    print("Let's go hiking")

else:
    print("Incorrect season input")

```
