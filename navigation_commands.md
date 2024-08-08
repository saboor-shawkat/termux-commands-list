# Navigation Commands in Termux

Navigating the filesystem efficiently is crucial when working in Termux. This document outlines common commands used to navigate directories and manage paths in Termux.

## Table of Contents

1. [Basic Navigation Commands](#basic-navigation-commands)
2. [Path Manipulation](#path-manipulation)
3. [Directory Operations](#directory-operations)
4. [Special Directories](#special-directories)

## Basic Navigation Commands

- `pwd`
  - Prints the current working directory.
  - Example: `pwd` (outputs the full path of the current directory).

- `ls`
  - Lists files and directories in the current directory.
  - Example: `ls` (lists files and directories).
  - Example: `ls -l` (lists in long format with detailed information).
  - Example: `ls -a` (lists all files including hidden files).

- `cd`
  - Changes the directory.
  - Example: `cd /data/data/com.termux/files/home` (navigates to the specified directory).
  - Example: `cd ..` (navigates up one level in the directory hierarchy).
  - Example: `cd ~` (navigates to the home directory).

## Path Manipulation

- `.` (dot)
  - Represents the current directory.
  - Example: `cd ./folder` (navigates to `folder` within the current directory).

- `..` (double dot)
  - Represents the parent directory.
  - Example: `cd ..` (moves up one directory level).

- `~` (tilde)
  - Represents the home directory of the current user.
  - Example: `cd ~/Documents` (navigates to the `Documents` directory in the home folder).

- `-` (dash)
  - Represents the previous directory.
  - Example: `cd -` (returns to the previous directory you were in).

## Directory Operations

- `mkdir`
  - Creates a new directory.
  - Example: `mkdir newdir` (creates a directory named `newdir`).

- `rmdir`
  - Removes an empty directory.
  - Example: `rmdir olddir` (deletes the `olddir` directory if it is empty).

- `rm -r`
  - Removes a directory and its contents recursively.
  - Example: `rm -r olddir` (deletes `olddir` and all files and directories within it).

- `mv`
  - Moves or renames files or directories.
  - Example: `mv oldname newname` (renames or moves `oldname` to `newname`).

- `cp`
  - Copies files or directories.
  - Example: `cp file.txt /path/to/destination/` (copies `file.txt` to the specified destination).

## Special Directories

- `/`
  - Represents the root directory of the filesystem.
  - Example: `cd /` (navigates to the root directory).

- `/sdcard/`
  - Represents the SD card or external storage.
  - Example: `cd /sdcard/Download` (navigates to the `Download` directory on the SD card).

- `/data/data/`
  - Represents the directory where Termux stores its data and applications.
  - Example: `cd /data/data/com.termux/files/home` (navigates to Termux's home directory).

## Conclusion

Mastering these navigation commands will help you manage and navigate your file system efficiently in Termux. For more details and options, refer to the respective command's manual page (e.g., `man cd`).

Happy navigating!

