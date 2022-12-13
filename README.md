# simple_shell

simple_shell is a basic UNIX command line interpreter, also known as a shell. It reads a command from the user and executes it using the `execve` system call. If the executable cannot be found, it prints an error message and displays the prompt again. It also handles the "end of file" condition (Ctrl+D) by printing a newline and exiting the program.

## Usage

To run `simple_shell`, compile the source code and run the resulting executable:

```
$ gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
$ ./hsh
```

## Examples

```
$ ./hsh
$ ls
hsh main.c shell.c
$ pwd
/home/vagrant/simple_shell
$ exit
$
```


Note that this implementation does not implement any advanced features, such as semicolons, pipes, redirections, or built-in commands. It also does not handle special characters, such as quotes, backslashes, or wildcards. Additionally, it does not search the `PATH` environment variable for the executable, so the user must specify the full path to the command.

## License

simple_shell is released under the MIT License. See the [LICENSE](LICENSE) file for details.
