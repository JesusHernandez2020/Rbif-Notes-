***Global Namespace:***

The global namespace is the top-level namespace that contains all the built-in names and global variables in your script.
Any variable or function declared at the top level of your script or module belongs to the global namespace.
Example:
```python

x = 10  # x is in the global namespace 
```
***Local Namespace:***

Each function or method creates its own local namespace, which contains variables defined inside that function.
Local variables can only be accessed within the function in which they are defined.
Example:
```python

def foo():
    y = 5  # y is in the local namespace of the function foo
```