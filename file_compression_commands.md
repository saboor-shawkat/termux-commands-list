# File Compression and Archiving Commands in Termux

File compression and archiving are essential for reducing file sizes and managing collections of files. This document provides an overview of common commands used to compress and archive files in Termux.

## Table of Contents

1. [Basic Compression Commands](#basic-compression-commands)
2. [Archive Creation](#archive-creation)
3. [Archive Extraction](#archive-extraction)
4. [File Compression Formats](#file-compression-formats)

## Basic Compression Commands

- `gzip`
  - Compresses files using the GNU zip compression algorithm.
  - Example: `gzip file.txt` (compresses `file.txt` to `file.txt.gz`).

- `gunzip`
  - Decompresses files compressed with `gzip`.
  - Example: `gunzip file.txt.gz` (decompresses `file.txt.gz` to `file.txt`).

- `bzip2`
  - Compresses files using the bzip2 compression algorithm.
  - Example: `bzip2 file.txt` (compresses `file.txt` to `file.txt.bz2`).

- `bunzip2`
  - Decompresses files compressed with `bzip2`.
  - Example: `bunzip2 file.txt.bz2` (decompresses `file.txt.bz2` to `file.txt`).

- `xz`
  - Compresses files using the xz compression algorithm.
  - Example: `xz file.txt` (compresses `file.txt` to `file.txt.xz`).

- `unxz`
  - Decompresses files compressed with `xz`.
  - Example: `unxz file.txt.xz` (decompresses `file.txt.xz` to `file.txt`).

## Archive Creation

- `tar`
  - Archives files into a single file.
  - Example: `tar -cvf archive.tar file1.txt file2.txt` (creates `archive.tar` containing `file1.txt` and `file2.txt`).
  - Example: `tar -cvf archive.tar directory/` (archives the contents of `directory/`).

- `tar.gz` or `tgz`
  - Creates a compressed archive using gzip.
  - Example: `tar -czvf archive.tar.gz file1.txt file2.txt` (creates a gzip-compressed archive).
  - Example: `tar -czvf archive.tgz directory/` (compresses `directory/` into `archive.tgz`).

- `tar.bz2`
  - Creates a compressed archive using bzip2.
  - Example: `tar -cjvf archive.tar.bz2 file1.txt file2.txt` (creates a bzip2-compressed archive).
  - Example: `tar -cjvf archive.tar.bz2 directory/` (compresses `directory/` into `archive.tar.bz2`).

- `tar.xz`
  - Creates a compressed archive using xz.
  - Example: `tar -cJvf archive.tar.xz file1.txt file2.txt` (creates an xz-compressed archive).
  - Example: `tar -cJvf archive.tar.xz directory/` (compresses `directory/` into `archive.tar.xz`).

## Archive Extraction

- `tar -xvf`
  - Extracts files from a tar archive.
  - Example: `tar -xvf archive.tar` (extracts files from `archive.tar`).

- `tar -xzf`
  - Extracts files from a gzip-compressed tar archive.
  - Example: `tar -xzf archive.tar.gz` (extracts files from `archive.tar.gz`).

- `tar -xjf`
  - Extracts files from a bzip2-compressed tar archive.
  - Example: `tar -xjf archive.tar.bz2` (extracts files from `archive.tar.bz2`).

- `tar -xJf`
  - Extracts files from an xz-compressed tar archive.
  - Example: `tar -xJf archive.tar.xz` (extracts files from `archive.tar.xz`).

## File Compression Formats

- **gzip**
  - File extension: `.gz`
  - Compression command: `gzip file.txt`

- **bzip2**
  - File extension: `.bz2`
  - Compression command: `bzip2 file.txt`

- **xz**
  - File extension: `.xz`
  - Compression command: `xz file.txt`

- **tar**
  - File extension: `.tar`
  - Archiving command: `tar -cvf archive.tar file.txt`

- **tar.gz (tgz)**
  - File extension: `.tar.gz` or `.tgz`
  - Compression command: `tar -czvf archive.tar.gz file.txt`

- **tar.bz2**
  - File extension: `.tar.bz2`
  - Compression command: `tar -cjvf archive.tar.bz2 file.txt`

- **tar.xz**
  - File extension: `.tar.xz`
  - Compression command: `tar -cJvf archive.tar.xz file.txt`

## Conclusion

Efficient file compression and archiving help manage disk space and simplify file transfers. For more detailed usage and options, refer to the respective command's manual page (e.g., `man tar` or `man gzip`).

Happy compressing and archiving!
