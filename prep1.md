**1. The Command Line:**
The command line is an interesting beast, and if you've not used one before, can be a bit daunting. Don't worry, with a bit of practice you'll soon come to see it as your friend. Don't think of it as leaving the GUI behind so much as adding to it.

**2. Basic Navigation:**

`pwd`
Print Working Directory - ie. Where are we currently.

`ls`
List the contents of a directory.

`cd`
Change Directories - ie. move to another directory.

**3. More About Files:**

`file`
obtain information about what type of file a file or directory is.

`ls -a`
List the contents of a directory, including hidden files.

**4. Manual Pages:**

`man <command>`
Look up the manual page for a particular command.

`man -k <search term>`
Do a keyword search for all manual pages containing the given search term.

`/<term>`
Within a manual page, perform a search for 'term'

`n`
After performing a search within a manual page, select the next found item.

**5. File Manipulation:**

`mkdir`
Make Directory - ie. Create a directory.

`rmdir`
Remove Directory - ie. Delete a directory.

`touch`
Create a blank file.
`cp`
Copy - ie. Copy a file or directory.

`mv`
Move - ie. Move a file or directory (can also be used to rename).

`rm`
Remove - ie. Delete a file.

**6. Vi Text Editor:**

`vi`
Edit a file.

`cat`
View a file.

`less`
Convenient for viewing large files.

**7. Wildcards:**

`Anywhere in any path`
Wildcards may be used at any part of a path.

`Wherever a path is used`
Because wildcard substitution is done by the system, not the command, they may be used wherever a path is used.

**8. Permissions:**

`chmod`
Change permissions on a file or directory.

`ls -ld`
View the permissions for a specific directory.

**9. Filters:**

`head`
View the first n lines of data.

`tail`
View the last n lines of data.

`sort`
Organise the data into order.

`nl`
Print line numbers before data.

`wc`
Print a count of lines, words and characters.

`cut`
Cut the data into fields and only display the specified fields.

`sed`
Do a search and replace on the data.

`uniq`
Remove duplicate lines.

`tac`
Print the data in reverse order.

**10. Grep and Regular Expressions:**

`egrep`
View lines of data which match a particular pattern.

`Regular Expressions`
A powerful way to identify particular pieces of information.

**11. Piping and Redirection:**

`>`
Save output to a file.

`>>`
Append output to a file.

`<`
Read input from a file.

`2>`
Redirect error messages.

`|`
Send the output from one program as input to another program.

**12. Process Management:**

`top`
View real-time data about processes running on the system.

`ps`
Get a listing of processes running on the system.

`kill`
End the running of a process.

`jobs`
Display a list of current jobs running in the background.

`fg`
Move a background process into the foreground.

`ctrl + z`
Pause the current foreground process and move it into the background.

**13. Scripting:**

`#!`
Shebang. Indicates which interpreter a script should be run with.

`echo`
Print a message to the screen.

`which`
Tells you the path to a particular program.

`$`
Placed before a variable name when we are referring to it's value.

``
Backticks. Used to save the output of a program into a variable.

`date`
Prints the date.

`if [ ] then else fi`
Perform basic conditional logic.

**14. Cheat Sheet:**
all above commands

