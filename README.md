# learning-python

What are Data Types and Variables? 

- No emphasis on declaring datatypes
- Three main data types 
    - Numbers 
    - Strings
    - Booleans 
- Variables can be used to give a name to data 
    - They are mutable -- can be updated and replaced 

- Numbers 
    - Three main types of numbers
        - Integer 
        - Floating Point Numbers 
        - Complex Numbers 
    - Integer 
        - Made up of positive + negative whole numbers 
        - Depending on the value of the integer, it will take up different amount of memory
            - ex: `0` -> 24 bytes, `1` -> 28 bytes 
    - Floating Point Numbers 
        - Made up of positive + negative decimal numbers 
        - Useful for precise calculations of values 
        - Takes up 24 bytes of memory 
    - Complex Numbers 
        - Numbers that are made up of real and an imaginary part. 
        - `complex(real, imaginary)` can be used to create complex numbers 
            - takes in two parts: real number and imaginary number
            - for imaginary, it will attach a `j` behind the imaginary argument that's passed in
        - Takes up 32 bytes of memory 

- Booleans 
    - bool 
    - has two values: `True` and `False`
    - useful to logic and data comparison 

- Strings 
    - collections of chracters enclosed by `""` or `''`
    - `len("will return the length of this string")`
    - indexing starts from zero 
    - each character can be accessed by enclosing the index with square brackets, `[]`
    - reverse indexing can be implemented by using a negative value, ex: `-1` refers to the last index of a string
    - string slicing: 
        - obtaining only a portion of the string
        - `string[start:end]`
            - the `start` is the index that you're starting from 
            - `end` is the index that you're ending at, not included. 
        - `string[start:end:step]`
            - skipping characters,`step` 
            - reverse slicing from the end to the front; the starting value is larger than the ending value and there must to be a negative value for the `step`
                - ex: `string[20:2:-1]`
            - partial slicing can happening if either the `start` or the `end` is left out 
                - if `start` is left out -- the slicing will start from the `0` index and stop at the `end` index
                - if `end` if left out -- the slicing will start  from the `start` index and end at the `n-1` index
        

