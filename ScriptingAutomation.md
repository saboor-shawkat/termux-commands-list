# Scripting and Automation Commands in Termux

Scripting and automation help streamline repetitive tasks and manage complex workflows. This document provides an overview of essential commands and tools for scripting and automation in Termux.

## Table of Contents

1. [Shell Scripting Basics](#shell-scripting-basics)
2. [Scheduling Tasks](#scheduling-tasks)
3. [Automation Tools](#automation-tools)
4. [Text Processing in Scripts](#text-processing-in-scripts)
5. [Error Handling and Debugging](#error-handling-and-debugging)

## Shell Scripting Basics

- `bash`
  - The Bourne Again Shell, a popular shell for scripting.
  - Example: `bash script.sh` (executes `script.sh` using `bash`).

- `#!/bin/bash`
  - Shebang line used to specify the script interpreter.
  - Example: `#!/bin/bash` (used at the beginning of a script to indicate it should be run with `bash`).

- `chmod +x`
  - Makes a script executable.
  - Example: `chmod +x script.sh` (sets the executable permission for `script.sh`).

- `echo`
  - Displays a message or variable value.
  - Example: `echo "Hello, World!"` (prints "Hello, World!" to the terminal).

- `read`
  - Reads user input.
  - Example: `read -p "Enter your name: " name` (prompts the user to enter their name).

## Scheduling Tasks

- `cron`
  - A daemon that executes scheduled commands.
  - Example: `crontab -e` (opens the cron table for editing).

- `crontab`
  - Manages cron jobs.
  - Example: `crontab -l` (lists current cron jobs).

- `at`
  - Schedules one-time tasks.
  - Example: `echo "bash script.sh" | at now + 1 minute` (runs `script.sh` in one minute).

- `sleep`
  - Pauses execution for a specified time.
  - Example: `sleep 60` (pauses for 60 seconds).

## Automation Tools

- `expect`
  - Automates interactive applications.
  - Example: `expect script.exp` (executes `script.exp` which automates interactions).

- `sed`
  - Stream editor for modifying text in scripts.
  - Example: `sed 's/old/new/g' file.txt` (replaces `old` with `new` in `file.txt`).

- `awk`
  - A powerful text processing language for scripting.
  - Example: `awk '{print $1}' file.txt` (prints the first field from each line in `file.txt`).

- `find`
  - Searches for files and directories and can execute commands on them.
  - Example: `find . -name "*.log" -exec rm {} \;` (finds and deletes all `.log` files).

## Text Processing in Scripts

- `grep`
  - Searches for patterns in files or input streams.
  - Example: `grep "pattern" file.txt` (searches for "pattern" in `file.txt`).

- `cut`
  - Extracts sections from each line of files.
  - Example: `cut -d: -f1 file.txt` (extracts the first field from lines in `file.txt`).

- `sort`
  - Sorts lines of text files.
  - Example: `sort file.txt` (sorts lines in `file.txt`).

- `tr`
  - Translates or deletes characters.
  - Example: `tr 'a-z' 'A-Z' < file.txt` (converts all lowercase letters to uppercase).

## Error Handling and Debugging

- `set -e`
  - Exits the script if any command fails.
  - Example: `set -e` (add to the script to stop on errors).

- `set -x`
  - Enables debugging mode to print commands and their arguments as they are executed.
  - Example: `set -x` (shows command traces during execution).

- `trap`
  - Executes commands when a script receives a signal.
  - Example: `trap 'echo "An error occurred"; exit 1' ERR` (executes on error).

## Conclusion

Scripting and automation improve efficiency and consistency in task management. For more detailed usage and options, refer to the respective command’s manual page (e.g., `man bash` or `man crontab`).

Happy scripting!
