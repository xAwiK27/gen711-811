

## Exercise

`echo` is a built-in shell command that writes its arguments, like a line of text to standard output.
The `echo` command can also be used with pattern matching characters, such as wildcard characters.
Here we will use the `echo` command to see how the wildcard character is interpreted by the shell.

```bash
$ echo *.fastq
```

```output
SRR097977.fastq SRR098026.fastq
```

The `*` is expanded to include any file that ends with `.fastq`. We can see that the output of
`echo *.fastq` is the same as that of `ls *.fastq`.

What would the output look like if the wildcard could *not* be matched? Compare the outputs of
`echo *.missing` and `ls *.missing`.



NAVIGATING PRACTICE
Navigate to your home directory. From there, list the contents of the untrimmed_fastq directory.

FINDING HIDDEN DIRECTORIES
First navigate to the shell_data directory. There is a hidden directory within this directory. Explore the options for ls to find out how to see hidden directories. List the contents of the directory and identify the name of the text file in that directory.

Hint: hidden files and folders in Unix start with ., for example .my_hidden_directory