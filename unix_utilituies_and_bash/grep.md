# grep is sort of like a search tool that matches a given patter or regular expression in a given file.
```bash 
grep "pattern" filename
```

## you can add many flags to grep to modify the search:

1. ```grep -i "pattern" filename``` -i makes grep case insentive.
2. ```grep -n "pattern" filename``` -n display the line number along with the matching lines 
3. ```grep -w "word" filename``` -w search for whole word only 
4. ```grep -v "pattern" filename``` -v show lines that does not match pattern 
5. ```grep -c "pattern" filename``` count the number of matching lines, ***note if you have the pattern in twice in a line,this would not be useful***

6. ```grep -r "pattern" filename``` matches directories 
7. ```grep -o "pattern" filename``` Use the -o option to show only the matching part of the lines:

8. To show lines of context around the matches, use the -A, -B, or -C options:

```-A ``` NUM: Show NUM lines after the match.

```-B``` NUM: Show NUM lines before the match.

```-C ```NUM: Show NUM lines of context around the match.
Example:
```bash 
grep -A 3 "error" log.txt
grep -B 2 "failed" log.txt
grep -C 5 "exception" log.t
```
***post assingment one here for clarification of how this works***

### all this flags can be combine to further custom the search, 
example:

```grep -o "error" | wc -l file ```

```grep -o "error"```: Extracts occurrences of the word "error".

```wc -l```: Counts the number of occurrences.

