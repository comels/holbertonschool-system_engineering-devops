# Project 0x02. Shell, I/O Redirections and filters

## About Bash projects

Unless stated, all your projects will be auto-corrected with Ubuntu 20.04 LTS.

## Resources

__Read or watch:__

    Shell, I/O Redirection
    Special Characters

__man or help:__

    echo
    cat
    head
    tail
    find
    wc
    sort
    uniq
    grep
    tr
    rev
    cut
    passwd (5) (i.e. man 5 passwd)

## Learning Objectives

At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

### Shell, I/O Redirection

    What do the commands head, tail, find, wc, sort, uniq, grep, tr do
    How to redirect standard output to a file
    How to get standard input from a file instead of the keyboard
    How to send the output from one program to the input of another program
    How to combine commands and filters with redirections

### Special Characters

    What are special characters
    Understand what do the white spaces, single quotes, double quotes, backslash, comment, pipe, command separator, tilde and how and when to use them

### Other Man Pages

    How to display a line of text
    How to concatenate files and print on the standard output
    How to reverse a string
    How to remove sections from each line of files
    What is the /etc/passwd file and what is its format
    What is the /etc/shadow file and what is its format

## Requirements

### General

    Allowed editors: vi, vim, emacs
    All your scripts will be tested on Ubuntu 20.04 LTS
    All your scripts should be exactly two lines long ($ wc -l file should print 2)
    All your files should end with a new line (why?)
    The first line of all your files should be exactly #!/bin/bash
    A README.md file, at the root of the folder of the project, describing what each script is doing
    You are not allowed to use backticks, &&, || or ;
    All your files must be executable
    You are not allowed to use sed or awk

## More Info

Read your /etc/passwd and /etc/shadow files.

Note: You do not have to learn about fmt, pr, du, gzip, tar, lpr, sed and awk yet.

## Task (mandatory)

| Task name | Description |
| --- | --- |
| 0. Hello World | Write a script that prints “Hello, World”, followed by a new line to the standard output. |
| 1. Confused smiley | Write a script that displays a confused smiley \"(Ôo)'. |
| 2. Let's display a file | Display the content of the /etc/passwd file. |
| 3. What about 2? | Display the content of /etc/passwd and /etc/hosts. |
| 4. Last lines of a file | Display the last 10 lines of /etc/passwd. |
| 5. I'd prefer the first ones actually | Display the first 10 lines of /etc/passwd. |
| 6. Line #2 | Write a script that displays the third line of the file iacta. The file iacta will be in the working directory. You’re not allowed to use sed. |
| 7. It is a good file that cuts iron without making a noise | Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line. |
| 8. Save current state of directory | Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it. |
| 9. Duplicate last line | Write a script that duplicates the last line of the file iacta.  The file iacta will be in the working directory. |
| 10. No more javascript | Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders. |
| 11. Don't just count your directories, make your directories count | Write a script that counts the number of directories and sub-directories in the current directory. The current and parent directories should not be taken into account. Hidden directories should be counted. |
| 12. What’s new | Create a script that displays the 10 newest files in the current directory. Requirements: One file per line and Sorted from the newest to the oldest. |
| 13. Being unique is better than being perfect | Create a script that takes a list of words as input and prints only words that appear exactly once. Input format: One line, one word. Output format: One line, one word. Words should be sorted. |
| 14. It must be in that file | Display lines containing the pattern “root” from the file /etc/passwd |
| 15. Count that word | Display the number of lines that contain the pattern “bin” in the file /etc/passwd |
| 16. What's next? | Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd. |
| 17. I hate bins | Display all the lines in the file /etc/passwd that do not contain the pattern “bin”. |
| 18. Letters only please | Display all lines of the file /etc/ssh/sshd_config starting with a letter. Include capital letters as well. |
| 19. A to Z | Replace all characters A and c from input to Z and e respectively. |
| 20. Without C, you would live in hiago | Create a script that removes all letters c and C from input. |
| 21. esreveR | Write a script that reverse its input. |
| 22. DJ Cut Killer | Write a script that displays all users and their home directories, sorted by users. Based on the the /etc/passwd file. |

## Task (advanced)

| Task name | Description |
| --- | --- |
| 23. Empty casks make the most noise  | Write a command that finds all empty files and directories in the current directory and all sub-directories. Only the names of the files and directories should be displayed (not the entire path). Hidden files should be listed.  One file name per line.  The listing should end with a new line.  You are not allowed to use basename, grep, egrep, fgrep or rgrep. |
|24. A gif is worth ten thousand words | Write a script that lists all the files with a .gif extension in the current directory and all its sub-directories. Hidden files should be listed. Only regular files (not directories) should be listed. The names of the files should be displayed without their extensions. The files should be sorted by byte values, but case-insensitive (file aaa should be listed before file bbb, file .b should be listed before file a, and file Rona should be listed after file jay). One file name per line. The listing should end with a new line. You are not allowed to use basename, grep, egrep, fgrep or rgrep. |
| 25. Acrostic | An acrostic is a poem (or other form of writing) in which the first letter (or syllable, or word) of each line (or paragraph, or other recurring feature in the text) spells out a word, message or the alphabet. The word comes from the French acrostiche from post-classical Latin acrostichis). As a form of constrained writing, an acrostic can be used as a mnemonic device to aid memory retrieval. Read more. Create a script that decodes acrostics that use the first letter of each line. The ‘decoded’ message has to end with a new line. You are not allowed to use grep, egrep, fgrep or rgrep. |