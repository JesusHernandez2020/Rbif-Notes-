# bash scripting

## How to run the script 

--> the file type is .sh

--> At the start of the script `#!/bin/bash`

--> to run the script, run the cmd: `bash` script.sh or use `chmod +x my_script.sh` to make it an executable. now you can run it as ./script.sh

## sintax

--> first important command, `echo`: output a string to the terminal example:

``` echo "hello word" ```

output: hello world

***variables***

--> same as any as any other programming language( ex python )
example 

```
name = john 

or 

path =home/project 

``` 

using the variables:



Definition: A variable is a container for storing data values. In bash, you can 
create a variable by using the syntax: `variable_name=value`. No spaces should be 
around the equal sign.

Accessing Variables: To access or use the value stored in a variable,
prefix its name with a dollar sign `$`. For example, if you define a variable 
myVar=10, you can access its value by typing `echo $myVar`.


```

cd $path   #move to the directory specify. 
```
you also use inputs and storage them in a variables by using `read`


```

echo what is your first name?

read FIRST_NAME 

echo what is your last name?

read LAST_NAME 

echo HELLO $FIRST_NAME $LAST_NAME

```
