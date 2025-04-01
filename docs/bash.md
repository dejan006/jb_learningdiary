# Bash
-----------------------------
Basic Commands:

| Command                       | Definition                                         |
|-------------------------------|----------------------------------------------------|
| pwd                           | shows current directory                            |
| ls                            | lists all files in current directory               |
| ls -l                         | lists all files with more details (rights, etc.)   |
| mkdir                         | create empty folder                                |
| rmdir                         | delete empty folder                                |
| touch                         | create file ("touch test.txt")                     |
| cat filename                  | shows contents of a file                           |
| cat filename filename2        | shows multiple files                               |
| rm                            | delete file                                        |
| rm -r foldername              | delete folder (-r = recursive)                     |
| mv                            | rename file / move file ("mv test.txt foldername") |
| mv -r                         | move folder ("mv foldername foldername2")          |
| echo                          | gives the echo back                                |
| echo "Hallo" > test.txt       | overwrites the file with "Hallo"                   |
| echo "Hallo" >> test.txt      | Adds "Hallo" to the file                           |
| ping url                      | test status of website                             |
| cp filename foldername        | copy file                                          |
| copy -r foldername foldername | copy folder                                        |
| if fi                         | syntax for if                                      |
| grep "text" test.txt          | search for something specific ("text") in a file   |
| history                       | command history                                    |
| clear                         | clear terminal                                     |

# Linux Man Pages – Quick Guide

Linux **man pages** (manual pages) are built-in documentation for commands, functions, config files, and more. You access them via the `man` command in the terminal.

## Basic Usage
```bash
man <command>
Example: man ls

## If Example
```bash
if [ Bedingung ]; then
  # Code 
fi

# Example
zahl=10
if [ "$zahl" -gt 5 ]; then
    echo "Die Zahl ist größer als 5"
fi
```