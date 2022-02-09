#!bins/bash
 __07th/February/2022__

__Learning more about text editors and shell scripts!__


"The following commands that make up the executable Scripts; __WRITE THEM WITHOUT THE FIRST AND LAST PARENTHESES!__"


0-hello_world (echo "Hello, World")

_Write a script that prints “Hello, World”, followed by a new line to the standard output._

1-confused_smiley (echo '"'"(Ôo)'")_

_Write a script that displays a confused smiley "(Ôo)'."_

10-no_more_js (find . -type f -name "*.js" -delete)

_Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders._

11-directories (find . -mindepth 1 -type d | wc -l)

_Write a script that counts the number of directories and sub-directories in the current directory._

12-newest_files (ls -t | head)

_Create a script that displays the 10 newest files in the current directory._

_Requirements:_

_1. One file per line_
_2. Sorted from the newest to the oldest_

13-unique (sort | uniq -u)

_Create a script that takes a list of words as input and prints only words that appear exactly once._

_1. Input format: One line, one word
_2. Output format: One line, one word
_3. Words should be sorted_

14-findthatword (grep root /etc/passwd)

_Display lines containing the pattern “root” from the file /etc/passwd_

15-countthatword (grep -c bin /etc/passwd)

_Display the number of lines that contain the pattern “bin” in the file /etc/passwd_

16-whatsnext (cat /etc/passwd | grep -A 3 "root")

_Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd_

17-hidethisword (grep -v bin /etc/passwd)

_Display all the lines in the file /etc/passwd that do not contain the pattern “bin”._

18-letteronly (grep ^[[:alpha:]]  /etc/ssh/sshd_config)

Display all lines of the file /etc/ssh/sshd_config starting with a letter.

_1. include capital letters as well_

19-AZ (tr 'Ac' 'Ze')

_Replace all characters A and c from input to Z and e respectively._

2-hellofile (cat /etc/passwd)

_Display the content of the /etc/passwd file_

20-hiago (tr -d 'Cc')

_Create a script that removes all letters c and C from input._

21-reverse (rev)

_Write a script that reverse its input._

22-users_and_homes (cut -d":" --fields=1,6 /etc/passwd | sort)

_Write a script that displays all users and their home directories, sorted by users._

_1. Based on the the /etc/passwd file_

3-twofiles (cat /etc/passwd /etc/hosts)

_Display the content of /etc/passwd and /etc/hosts_

4-lastlines (tail -n10 /etc/passwd)

_Display the last 10 lines of /etc/passwd_

5-firstlines (head -n10 /etc/passwd)

_Display the first 10 lines of /etc/passwd_

6-third_line (head -n 3 iacta | tail -n 1)

_Write a script that displays the third line of the file iacta._

_The file iacta will be in the working directory_

_1. You’re not allowed to use sed_

7-file (echo "Best School" | cat > '\*\\'\''"Best School"\'\''\\*$\?\*\*\*\*\*:)')

_Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line._

8-cwd_state (ls -la > ls_cwd_content)

_Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it._

9-duplicate_last_line (echo | tail -n1 iacta >> iacta)

_Write a script that duplicates the last line of the file iacta_

_The file iacta will be in the working directory_
