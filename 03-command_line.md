# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > Commands
>> >> show current working directory path
>> >> ``` console 
>> >> pwd 
>> >> ```
>> >> creating a directory
>> >> ``` console
>> >> mkdir <directory_name>
>> >> ```
>> >> deleting a directory
>> >> ``` console
>> >> rm +r <directory_name>
>> >> ```
>> >> creating a file using `touch` command
>> >> ``` console
>> >> touch <file_name>
>> >> ```
>> >> deleting a file
>> >> ``` console
>> >> rm <file_name>
>> >> ```
>> >> renaming a file
>> >> ``` console
>> >> 
>> >> ```
>> >> listing hidden files
>> >> ``` console
>> >> ls -a
>> >> ```
>> >> copying a file from one directory to another
>> >> ``` console
>> >> cp <file_name> <destination_directory_name>
>> >> ```
>> >> searching for a particular file using grep
>> >> ``` console
>> >> 
>> >> ```

> > 
---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t` 
`ls -Glp`  

> > 
>> >> ```console
>> >> ls
>> >> ```
>> >> lists all the files and directories(excluding the hidden ones) in the particular/working directory
>> >> ```console
>> >> ls -a
>> >> ```
>> >> lists all the files and directories in the particular/working directory
>> >> ```console
>> >> ls -l
>> >> ```
>> >> lists all the files along with their user details etc (i.e. in the long format)
>> >> ```console
>> >> ls -lh
>> >> ```
>> >> lists the files and directories in the long format with the size mentioned in human-readable format like Bytes,GB etc
>> >> ```console
>> >> ls -lah
>> >> ```
>> >> lists the files and directories(including hidden ones) in the long format with the size mentioned in human-readable format like Bytes,GB etc
>> >> ```console
>> >> ls -t
>> >> ```
>> >> lists the files in the descending order of when they have been modified
>> >> ```console
>> >> ls -Glp
>> >> ```
>> >> lists the files and directories in the long format. Highlights the directories by using a '/' at the end of the directory name
> > 
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > My favorites:
>> >> ```console
>> >> ls -a
>> >> ```
>> >> displays all the files and directories including the hidden ones
>> >>```console
>> >> ls -alt
>> >> ```
>> >> displays all the files and directories including the hidden ones based on the time of modification of the files
>> >>```console
>> >> ls -R
>> >> ```
>> >> displays the contents of the sub directories as well
>> >>```console
>> >> ls -l
>> >> ```
>> >> displays the details of the files and directories in the long format
>> >>```console
>> >> ls -lh
>> >> ```
>> >> lists the files and directories in the long format with the size mentioned in human-readable format like Bytes,GB etc
---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > 'xargs' is a UNIX command which processes a long list of file names. It can be used in conjunction with the "find" and "grep" commands.For example :
>> >> ``` console
>> >> find ./python -print | xargs grep "match_ends"
>> >> ```
>> >> This Command would return all the lines in the files in python directory where the word "match_ends" is present.
 

