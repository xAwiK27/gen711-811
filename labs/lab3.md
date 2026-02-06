# Lab3 - 2/6/26

## Before lab begins
1. Open up vscode
2. Control + shift + 'p' to open command prompt (command + shift + p on apple)
3. Start typing 'Connect to...' and the 'Connect current window to host' menu item will pop up. Select it
4. If asked, connect to 'ron.sr.edu host'
5. Enter your RON username if prompted
6. Enter your RON password when prompted
7. Go to 'File --> Open folder'
8. Select your 'gen711-811' directory
9. If you haven't done so already, save your workspace to this directory (File --> save directory as --> enter)
10. Take your notes in 'Markdown' format. See the readme.txt for taking notes for this lab below. 

### Your Notes Here: 
Seperate notes by an empty line, or they'll get pasted together

- Using a dash is helpful for lists
1. And numbers for lists

The pound sign is used for 'sections'. A single pound (or hashtag) in front of a word makes it appear bigger/bold to show a new section. See below

# My Notes:

To change directories, use 'cd' and then hit tab two times to see directories in my current directory
pwd (print working directory) --> lists current directory location
ls (lists 'things' in directory: -F = folders/directories, -lrth prints information about ownership/perms, putting a * matches specific search to desired thing)
man (command here) (full operating manual for command)
head (prints ~10x lines to the screen)
cd .. (back out of directory- can do multiple times separated by a '/' to continuously back out to home directory)
conda = environment manager w/ extra stuff (unnecessary for the time being- but information nonetheless)
rm -fR (directory)dir (removal of directory and all of its files)
git clone (ADDRESS) (cloning a repository from github)
using a dollar sign specifies variable
grep (search for) (file search in) --> search through file and return the lines that match the search query ('@' no quotes is a special character, ^ is also a special character- specifies that it is the beginning of the line)
grep '@SRR097977' SRR097977.fastq > headerlines.txt (moves stuff desired to a new file)
pipe special character ( | ) --> sends command to another command
ls /bin | grep -iE 'a|c' (send search to bin, find files with a or c within it)
less (file_name) --> can scroll through entire file to view it

### Complete the questions below when intrstructed. Push the changes to this document to recive credit for attending the lab

#### 1. What are 3 ways to change directories to your home directory from the  untrimmed_fastq directory?
1. cd home/users/USERNAME
2. cd ~
3. cd $HOME
4. cd ../../../

#### 3b. How many programs in /bin 
2. Do each of the following tasks from your current directory using a single ls command for each:
    - List all of the files in /bin that start with the letter ‘c’.
    - List all of the files in /bin that contain the letter ‘a’.
    - List all of the files in /bin that end with the letter ‘o’.
    - Bonus: List all of the files in /bin that contain the letter ‘a’ or the letter ‘c’ > ls /bin | grep -iE 'a|c'

#### Answers here
Start with the letter c > ls c*
Start with the letter a > ls -F *a
Start with the letter o > ls o*
Contain the letter ‘a’ or the letter ‘c’ >

#### What command/commands would you use to find the line number in your history for the command that listed all the '.fastq' files using the absolute path. Paste your answer below.
ls *fastq