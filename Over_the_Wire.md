#Linux for Cybersecurity

Today I used Linux to access Bandit's hostname in Over The Wire, a game for learning Linux. 
I basically learned to use the commands ls, cd, cat, file, du, and find.

#Practice
During this process, I used ls to view the folders in the root directory, 
then cat to print the contents of the file. I used cat ./- when the file name was a hyphen, 
which Linux finds confusing. Finally, I used find to locate a hidden file inside a 
folder that couldn't be accessed with a simple cat command. So what I did was 
use `file` and `medio`, which was a directory file, and then I used `cd` to enter it, 
then `find` to search its contents, and finally `cat ./`, which gave me the password 
and allowed me to access the next Bandit files. With `file`, I was able to see the content
type of each file from the terminal, inside another folder with hidden files. 
Some were binary data, others public keys, but I finally found the "ASCII text" file, 
which was the right one. That's basically what I achieved today on this page.

