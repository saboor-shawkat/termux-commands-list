# Security and Permissions Commands in Termux

Security and permissions commands are essential for managing access rights and ensuring the safety of your files and system. This document provides an overview of commands used for security and permissions management in Termux.

## Table of Contents

1. [File Permissions](#file-permissions)
2. [User and Group Management](#user-and-group-management)
3. [System Security](#system-security)
4. [Network Security](#network-security)
5. [File Integrity](#file-integrity)

## File Permissions

- `chmod`
  - Changes file permissions.
  - Example: `chmod 755 file.txt` (sets read, write, and execute permissions for the owner, and read and execute permissions for others).

- `chown`
  - Changes file owner and group.
  - Example: `chown user:group file.txt` (changes the owner of `file.txt` to `user` and the group to `group`).

- `chgrp`
  - Changes group ownership of a file.
  - Example: `chgrp group file.txt` (changes the group of `file.txt` to `group`).

- `umask`
  - Sets default permission mask for new files and directories.
  - Example: `umask 022` (sets the default permissions for new files to `644` and directories to `755`).

## User and Group Management

- `useradd`
  - Adds a new user to the system.
  - Example: `useradd username` (creates a new user `username`).

- `usermod`
  - Modifies user account properties.
  - Example: `usermod -aG group username` (adds `username` to `group`).

- `userdel`
  - Deletes a user account.
  - Example: `userdel username` (deletes the user `username`).

- `groupadd`
  - Adds a new group to the system.
  - Example: `groupadd groupname` (creates a new group `groupname`).

- `groupdel`
  - Deletes a group.
  - Example: `groupdel groupname` (deletes the group `groupname`).

## System Security

- `sudo`
  - Executes commands with superuser privileges.
  - Example: `sudo command` (runs `command` as the superuser).

- `passwd`
  - Changes user passwords.
  - Example: `passwd username` (changes the password for `username`).

- `sudoers`
  - Configures user privileges for `sudo` (requires editing `/etc/sudoers`).
  - Example: `visudo` (opens the sudoers file for editing).

- `pkill`
  - Sends signals to processes based on name.
  - Example: `pkill -9 processname` (forcefully terminates `processname`).

- `kill`
  - Sends signals to processes by PID.
  - Example: `kill -9 1234` (forcefully terminates the process with PID `1234`).

## Network Security

- `iptables`
  - Configures network packet filtering rules.
  - Example: `iptables -A INPUT -p tcp --dport 22 -j ACCEPT` (allows incoming SSH connections on port 22).

- `nmap`
  - Scans networks for open ports and services (requires installation).
  - Example: `nmap 192.168.1.1` (scans the IP address `192.168.1.1` for open ports).

- `ufw`
  - Manages a firewall (requires installation).
  - Example: `ufw enable` (enables the firewall).

- `ssh`
  - Securely connects to remote systems over SSH.
  - Example: `ssh user@hostname` (connects to `hostname` as `user`).

## File Integrity

- `md5sum`
  - Computes and verifies MD5 checksums.
  - Example: `md5sum file.txt` (computes the MD5 checksum of `file.txt`).

- `sha256sum`
  - Computes and verifies SHA-256 checksums.
  - Example: `sha256sum file.txt` (computes the SHA-256 checksum of `file.txt`).

- `tripwire`
  - Monitors file integrity (requires installation and configuration).
  - Example: `tripwire --check` (checks file integrity against a database).

## Conclusion

Managing security and permissions is crucial for protecting your system and data. For more detailed usage and options, refer to the respective command’s manual page (e.g., `man chmod` or `man iptables`).

Stay secure!
