# Functions are a powerful tool to help write cleaner code. If you find yourself writing the same block of statements over and over again, this could be defined in a function, and then all you would have to do is execute the function instead of copy pasting lines of code.


***defining a function***
first call the key word ```def ``` and you name of the funtion follow by parenthesis. you can either define the function without argument or with arguments like i did below. 

```an argument``` is basically an input value you have to give the function 

***Calling a Function***
After defining a function, you can call it by using its name followed by parentheses. Pass the required arguments inside the parentheses.


```python 
def lower_case(var):

	return var.lower() 

print(lower_case("ATCGATCGCGTA")) #this  is called calling the function ATCGATCGCGT is our argument 
```
***output***: atcgatcgcgta

you can use the funciton to ouput lowercase of any string


```return``` this is a key word we use to return a value, in this case im telling the function to give me ```var``` our the string im inputing when i called the function and modifying to lower case by using ```lower()``` which is a built in function in python 


### another example with parameter 
```python
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()          # Output: Hello, Guest!
greet("Bob")     # Output: Hello, Bob!
```


## more about functions 
this docs will be updated as i learn more about functions


