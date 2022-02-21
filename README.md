# Homework_2
To implement a search program in C program using system calls for files and 
directories. 

# description
1. The program  takes the directory name from where to start the file traversal as a 
command-line argument and print the file hierarchy starting with the directory that is 
provided by the command-line argument. 
2. If the program is executed without any arguments, the program should print the file 
hierarchy starting with the current directory where the program is executed. If there are no 
directories in the current directory only files are listed one per line. 
3. If there are other directories in the current directory then the directory name is first 
displayed on a separate line and then the files in that directory are listed one-per-line with 
one-tab indentation. 
4. If a file is a symbolic link then the program should display the symbolic link name and in 
parentheses the file name the link points to. 
5. The program should also support three command-line options: 
1. -S 
This should list all files in the file hierarchy and print the file size next to the filename in 
parenthesis.  
2. -s <file size in bytes> 
This should list all files in the file hierarchy with file size greater than or equal to the 
value specified. 
3. -f <string pattern> 
This should list all files in the file hierarchy whose file name or directory name contains 
the substring specified in the string pattern option. 
6. The program should support not only each of these options separately but also any 
combination of these options. For example: -S, -s 1024, -f jpg, -S -s 1024, -S -f jpg, -s 
1024 -f jpg, -S -s 1024 -f jpg, -S -f jpg -s 1024. 
7. If both -s and -f options are specified then the program should list only those files that 
match both criteria. The order of the options should not matter. 
8. -t d will display the directories
  -t f will display all the files

# Getting started
These instructions will give you a copy of the project up and running on your local machine for development and testing purposes.
# prerequisites
Requirements for the software and other tools to build, test and push
1. gcc - GNU Compiler Collection
2. Text editor

# installing
A step by step series of examples that tell you how to get a development environment running
1. open the text editor
2. create a c programming file
3. save the file with .c extension.

# Running the tests

functionality of the program:

It uses switch method to take input from command line arguments
  Depending on the input, it goes to a function name printFileHierarchy
  and prints the required ouput based on the command line arguments.
  
  if -s 1022 is given, it displays the files with size>0 1022
  if -f 'abc' is given, it displays the files with substring 'abc'
  if -S is given it displays the files and its size.
  
  ALl the other combinatios are also given as input.


In the int main(), these methods are called at the right time. 


In general a c program is executed in this way:
1. To compile the file, type the command 'gcc filename.c'
2. To run the file, type './a.out'

To test our program, follow the below steps

1. gcc sample.c 
2. ./a.out <path>
    
output: 
```To send a file in input stream, follow the below steps:
 ./a.out /Users/rnvsrivastava/projects
[1] .DS_Store (size:8196)
[1] .DS_Store (8196)
[2] project1 (128)
[1] README (size:0)
[1] README (0)
[2] project1.docx (size:0)
[2] project1.docx (0)
[3] read.c (size:0)
[3] read.c (0)
[4] fread.c (size:0)
[4] fread.c (0)
[5] project3 (128)
[1] project3.docx (size:0)
[1] project3.docx (0)
[2] README (size:0)
[2] README (0)
[6] project4 (128)
[1] project4.docx (size:0)
[1] project4.docx (0)
[2] README (size:0)
[2] README (0)
[7] project2 (128)
[1] project2.docx (size:0)
[1] project2.docx (0)
[2] README (size:0)
[2] README (0)
[8] write.c (size:0)
[8] write.c (0)
[9] fwrite.c (size:0)
[9] fwrite.c (0)
```
# Author
Sri Vastava RNV

# Acknoledgement

I thank my TA's and Dr. Mahmut Unan for helping me learn everyday. 


