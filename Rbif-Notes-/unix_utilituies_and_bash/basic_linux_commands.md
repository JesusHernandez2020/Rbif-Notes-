# here are some basic commands to know as you navigate the terminal 

1. ```cd ```
    this command you can can use to change directory 
    for example you in ```user/home```
    you can say ```cd user/home/desktop``` to switch desktop, you can also use ```cd -``` to go back to the previous directory 
    


2. ```pwd```

    to print the current working directory.
    ```C:\Users\Jesus\OneDrive\Desktop\Rbif-Notes-``` is th location of this file when i type ```pwd``` in the terminal 
    ***note: rembember the difference of relative vs absolute path***

3. ```mkdir``` new_directory

4. ```rm ```file.txt what out becareful if rm files you can recover them 
5. ```rm ``` -r directory_name 

6. ```cp source_file.txt destination_file.txt```: copies a file to another directory
      
      
    **interesting uses of cp**
    
    **a**. The cp -R command is used to copy directories and their contents recursively 
    in a Unix-like operating system. Here’s a breakdown of how it works:
      
      **Command Structure:**
      The command consists of cp, which stands for copy, 
      followed by the -R (or --recursive) flag, the source directory, and the destination.
      The syntax is:
      
      ```cp -R [source_directory] [destination_directory]```
      
      
      
  
      **Recursive Copying:**
      
      The -R flag instructs the cp command to copy not just the directory but 
      also all its subdirectories and the files within them. 
      This creates an exact replica of the entire directory structure at the target location.
  
      **Example Usage:**
      
      lets say we want to copy a directory named documents to a new directory 
      called documents_backup, you would run:
              
      `cp -R documents/ documents_backup/`
      
      

    **b**. ```cp -r source_directory destination_directory``` copies a directory to another dir. ***note: new command, i did not know.***
  
  
  
7. ```mv``` move a file from a destination to another, can also be use to rename files. mv ```old_name.txt new_name.txt``` renaming a file 
``` mv file.txt /path/to/destination/``` moving a file 
***note this is also use in ssh servers but as ```scp```

8. ```cat```: Concatenates and displays file contents.```cat file.txt``` displays the content of file.txt on to the terminal. ***you can use cat>>file to output data into a file**

9. `mkdir`

    used to create new directories in a Unix-like operating system. 
    
    ```mkdir newdir```
    
    you can also create You can also create multiple directories in one command:
    
    ```mkdir dirone dirtwo dirthree```
    
    one last cool thing is that If you want to create nested directories and some
    parent directories do not exist, you can use the `-p` option:
    
    **example**
    ```mkdir -p parent_dir/child_dir/grandchild_dir```

  

## notes from udemy course 

## this is for file filtering 

`file globbing` is a powerful feature in the shell that uses wildcard characters
to match groups of files. Here are the key concepts related to file globbing:

Wildcard Characters:
`Asterisk *`: This represents any number of characters. For example, using
`ls *.txt` will list all .txt files in the current directory.
`Question Mark ?`: This represents a single character. For example, 
`ls file?.txt` will look for files like file1.txt or fileA.txt, but not file12.txt.
`Brackets []`: You can specify a range of characters. For instance, 
`ls file[a-i].txt` will match filea.txt to filei.txt.

Exclusion:
You can also exclude certain patterns using `!`. For example,
ls file[!a].txt will match all files except those starting with 'a'.

Examples of Usage:
To see all files in a directory using wildcards, you might use a command 
like `ls -l *`, which will display all files.
If you want to copy all files from a directory into your current directory, 
you might use `cp /path/to/documents/*` .. Here, the asterisk grabs all files 
from the specified directory.

Practical Applications:
File globbing can be especially useful for performing bulk file operations, 
such as moving or renaming multiple files at once.

Understanding and mastering file globbing will significantly enhance your efficiency
in navigating and managing files in a shell environment. If you have any specific 
scenarios or further questions, feel free to ask!
Was this content relevant to you?



