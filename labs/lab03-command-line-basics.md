Lab 3: Command Line Basics
================
Gaston Sanchez

> ### Learning Objectives
>
> -   Practicing with the command line
> -   Navigating the filesystem and managing files
> -   Practice basic manipulation of data files

------------------------------------------------------------------------

Basic Bash shell commands
-------------------------

The first part of the lab involves navigating the file system and manipulating files (and directories) with the following basic bash commands:

-   `pwd`: print working directory
-   `ls`: list files and directories
-   `cd`: change directory (move to another directory)
-   `mkdir`: create a new directory
-   `touch`: create a new (empty) file
-   `cp`: copy file(s)
-   `mv`: rename file(s)
-   `rm`: delete file(s)

If you are using git-bash (i.e. your OS is Windows) you don't have the `man` command to see the manual documentation of other commands. In this case you can check the *man* pages online:

<http://man7.org/linux/man-pages/index.html>

Your turn
---------

Write your bash commands in a text editor (NOT a word processor) and save them in a text file: e.g. `lab03-gaston-sanchez.txt`.

-   Open (or launch) the command line
-   Use `mkdir` to create a new directory `stat133-lab03`
-   Change to the directory `stat133-lab03`
-   Use the command `curl` to download the following text file:

    ``` bash
    # the option is the letter O (Not the number 0)
    curl -O http://textfiles.com/food/bread.txt
    ```

-   Use the command `ls` to list the contents in your current directory
-   Use the command `curl` to download these other text files:
    -   <http://textfiles.com/food/btaco.txt>
    -   <http://textfiles.com/food/1st_aid.txt>
    -   <http://textfiles.com/food/beesherb.txt>
-   Use the command `curl` to download the following csv files:
    -   <http://archive.ics.uci.edu/ml/machine-learning-databases/forest-fires/forestfires.csv>
    -   <http://www.math.uah.edu/stat/data/Fisher.csv>
    -   <http://web.pdx.edu/~gerbing/data/cars.csv>
-   Now try `ls -l` to list the contents in your current directory in long format
-   Look at the `man` documentation of `ls` to find out how to list the contents in reverse order
-   How would you list the contents in long format and by time?
-   Inside `stat133-lab03` create a directory `data`
-   Change to the directory `data`
-   Create a directory `txt-files`
-   Create a directory `csv-files`
-   Use the command `mv` to move the `bread.txt` file to the folder `txt-files`
-   Use the wildcard `*` to move all the text files to the directory `txt-files`
-   Use the wildcard `*` to move all the `.csv` files to the directory `csv-files`
-   Go back to the parent directory `stat133-lab03`
-   Create a directory `copies`
-   Use the command `cp` to copy the `bread.txt` file (the one inside the folder `txt-files`) to the `copies` directory
-   Use the wildcard `*` to copy all the `.txt` files in the directory `copies`
-   Use the wildcard `*` to copy all the `.csv` files in the directory `copies`
-   Change to the directory `copies`
-   Use the command `mv` to rename the file `bread.txt` as `bread-recipe.txt`
-   Rename the file `Fisher.csv` as `iris.csv`
-   Rename the file `btaco.txt` as `breakfast-taco.txt`
-   Change to the parent directory (i.e. `stat133-lab03`)
-   Rename the directory `copies` as `copy-files`
-   Find out how to use the `rm` command to delete the directory `copy-files`
-   List the contents of the directory `txt-files` displaying the results in reverse (alphabetical) order

### Optional challenge

If you are already familiar with the basic bash commands to navigate the filesystem (or if you want to expand your R skills), use the R functions to manipulate files and directories to perform the exact same tasks from within R. See `?files` for more information.

-   `getwd()`
-   `setwd()`
-   `download.file()`
-   `dir.create()`
-   `list.files()`
-   `list.dirs()`
-   `file.create()`
-   `file.copy()`
-   `file.rename()`
-   `file.remove()`

------------------------------------------------------------------------
