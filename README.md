# xv6-tail

## Implementing the 'tail' command
Write a program that prints the last 10 lines of its input. If a filename is provided on the command line (i.e., tail FILE ) then tail should open it, read and print the last 10 lines, and then close it. If no filename is provided, tail should read from standard input.

The traditional UNIX tail utility can print out a configurable number of lines from the start of a file. Implement this behavior in your version of tail . The number of lines to be printed should be specified via a command line argument as tail -NUM FILE , for example tail -3 README to print the last 3 lines of the file README. If the number of lines is not given (i.e., if the first argument does not start with - ), the number of lines to be printed should default to 10 as in the previous part.

Hints:
1. Many aspects of this are similar to the wc program: both can read from standard input if no arguments are passed or read from a file if one is given on the command line. Reading its code will help you if you get stuck.
2. You can convert a string to an integer with the atoi function.
3. You may want to use pointer arithmetic (discussed in class in Lecture 2) to get a string suitable for passing to atoi .
