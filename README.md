# Bash file tutorial

## Chapter 1: Hello world

### Commands
- `pwd`: Prints the name of the current working directory
- `cd`: Changes the shell’s working directory
- `echo`: Prints its arguments separated by a space and terminated by
a newline
- `type`: Displays information about a command
- `mkdir`: Creates a new directory
- `chmod`: Modifies the permissions of a file
- `source`: a.k.a. .(dot), executes a script in the current shell
environment
- `printf`: Prints the arguments as specified by a format string

### Concepts
- `Script`: A file containing commands to be executed by the shell.
- `Word`: A word is a sequence of characters considered to be a single
unit by the shell.
- `Output redirection`: The output of a command can be sent to a file
rather than the terminal using `> FILENAME`.
- `Variables`: These are the names where values are stored
- `Comments`: These consist of an unquoted word beginning with a #.
All remaining characters on that line constitute a comment and will
be ignored.
- `Shebang` or `hash-bang`: This is a hash and an exclamation mark (#!)
Dùng để chỉ đường cho trình thông dịch (Interpreter). Ký hiệu này giúp hệ điều hành biết cách thực thi mã nguồn mà không cần phải gõ trực tiếp vào dòng lệnh.

### Variable
- `PWD` contains the pathname of the shell’s current working directory.
- `HOME` stores the pathname of the user’s home directory.
- `PATH` is a colon-separated list of directories in which command files are stored. The shell searches the directories for commands it is asked to execute.

## Chapter 2: “Input, Output, and Throughput”

### Parameters and Variables

- A parameter is an entity to store values
- There are three types of parameters:
  - `positional parameters`: are aguments present on the command line
  - `special parameters`: are set by the shell to store infomation about aspects of its current state, such as the number of arguments and the exit code of the last command
  - `variables`: are identified by a name

