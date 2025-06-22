# grep is sort of like a search tool that matches a given patter or regular expression in a given file.
```bash 
grep "pattern" filename
```

## you can add many flags to grep to modify the search:
```grep pattern * ``` search for files that contain pattern 

0.```grep -e"pattern 1" -e"pattern 2" file``` can search multiple pattern 

1. ```grep -i "pattern" filename``` -i makes grep case insentive.
2. ```grep -n "pattern" filename``` -n display the line number/s where the matching pattern is found
3. ```grep -w "word" filename``` -w search for whole word only 
4. ```grep -v "pattern" filename``` -v show lines where the pattern does not exist
5. ```grep -c "pattern" filename``` count the number of matching lines,**not how many times on a line**


6. ```grep -r "pattern" filename``` matches directories 
7. ```grep -o "pattern" filename``` Use the -o option to show only the matching part of the lines: **can be pipe 
to wc to find out the number of occurrences of pattern in a file(useful for motif finding in fasta files, example grep -o atg |wc)**

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

