## Data Types and Variables

* No emphasis on declaring datatypes
* Three main data types 
    * Numbers 
    * Strings
    * Booleans 
* Variables can be used to give a name to data 
    * They are mutable -- can be updated and replaced 

### Numbers

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


