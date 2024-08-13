Repetitive execution of the same block of code over and over is referred to as ***iteration.***
There are two types of ***iteration***:
***Definite iteration***, in which the number of repetitions is specified explicitly in advance
***Indefinite iteration***, in which the code block executes until some condition is met
In Python, ***indefinite iteration*** is performed with a while loop.


***Definite iteration*** loops are frequently referred to as `for `loops because for is the keyword that is used to introduce them in nearly all programming languages, including Python.

Python’s for loop looks like this:

```python
for <var> in <iterable>:
    <statement(s)>```

`<iterable>` is a collection of objects—for example, a `list` or `tuple.` The <statement(s)> in the loop body are denoted by indentation, as with all Python control structures, and are executed once for each item in <iterable>. The loop variable <var> takes on the value of the next element in <iterable> each time through the loop.

Example: How to count the number of adenines in a specific DNA sequence
```python
a_counter = 0
long_sequence = “”
for DNA_sequence in list_of_sequences:
     long_sequence = long_sequence + DNA_sequence 
     for each_nt in DNA_sequence:
           if each_nt == “A”:
                  print(“This is adenine”)
                  a_counter += 1
           elif each_nt == “M”:
                  print(“This is not a valid DNA base”)
print(“There are “ + str(a_counter) + “ adenosine bases”)
```