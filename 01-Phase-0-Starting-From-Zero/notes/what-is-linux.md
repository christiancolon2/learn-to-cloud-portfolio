<p align="center">
  <img src="/00-Start-Here/Images/banner.png" width="900">
</p>

# What is Linux

## Bash Scripting and Command Line for Beginners

- **Bash Script** - is a file that stores a list of commands for your computer to run.
- The Bash program reads the file and runs each command one by one. No need to type the commands repeatedly. Just save them in a script and run it whenever you need to.

### Advantages of Bash Scripting

- **Automation** - Lets you automate repetitive tasks.
- **Portability** - Work on many systems like Linux, macOS, and Windows.
- **Flexibility** - You can easily change scripts to fit your needs.
- **Accessibility** -You only need a basic text editor to write a script.
- **Integration** - Can work with other tool like databases, servers, and cloud services.
- **Debugging** - It's easy to find and fix errors when something goes wrong.

### Bash Shell and Command Line Interface

- **Shell** - is a program that lets you control your computer using typed commands.
- **Bash** - is a type of shell. It's the default shell on many linux systems.
- When you use a shell, you see a prompt like this:
  - **$** - means you are a normal user.
  - **#** - means you are the root (admin) user.
- So:
  - **Shell** - general name for command line programs
  - **Bash** - a specific and very popular shell
- **ps** - command lets you know the type of shell you are using.

![ps command results](/01-Phase-0-Starting-From-Zero/screenshots/ps-command-results.png)

- **Commands** follow the this syntax:

```bash
command [OPTIONS] arguments
```

- **date** - displays the current date

```bash
zaira@Zaira:~/shell-tutorial$ date
Tue Mar 14 13:08:57 PKT 2023
```

- **pwd** - shows the current folder (directory) you are in.

```bash
zaira@Zaira:~/shell-tutorial$ pwd
/home/zaira/shell-tutorial
```

- **ls** - shows the files and folders inside the current directory

```bash
zaira@Zaira:~/shell-tutorial$ ls
check_plaindrome.sh  count_odd.sh  env  log  temp
```

- **echo** - used to display messages or output words on the command line

```bash
zaira@Zaira:~/shell-tutorial$ echo "Hello bash"
Hello bash
```

- **man** - shows the help page for a comman. The page explains what the command does and how to use it.

- **shebang** - is the first line in a script that tells the system which program should run the script.
  - **#!** tells the system this is a shebang line.
  - **/bin/bash** tells the system to run the script using Bash.

- **which** - shows the location of a command's program file on your system.

- **vi** lets your create, view, and edit files directly in the terminal.
- **#** - starts a comment. Anything after **#** is ignored by the computer. It is only for humans to read.

- **Variable** - is a name used to store a value.

```bash
name="Chris"
```

### Variable Naming Rules

- Variable names must start with a letter or underscore
- They can include letters, numbers, and underscores
- Variable names are case sensitive, so **name** and **Name** are different.
- Variable names cannot have spaces or special characters
- Use clear names that describe what the variable stores
- Do not use Bash words like if, then, else or fi as variable names.

- **read** - is a bash command that takes input from the user or from a file and stores it in a variable.
