#conditional statements

###pretty simple:

if a test is true do something, else do something else;
***below is an example***
```python 
if “ATT” in sequence:

     print(“This is an ATT present”)
elif “GC” and “ATT” in sequence: #Why would this statement *never* be evaluated a True?
     print(“There is a GC and ATT present”)	
else:
      print(“Neither ATT nor GC is present”)
*Note 1* in is an operator that tests for membership, usually used to test if you are looking for a substring of a string. 
*Note 2* and and or are logical operators and can be used to test for multiple conditions at once.
```