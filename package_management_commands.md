# Package Management Commands in Termux

Termux uses a package management system to handle software installation and updates. This document provides an overview of common package management commands in Termux.

## Table of Contents

1. [Basic Package Management Commands](#basic-package-management-commands)
2. [Package Installation](#package-installation)
3. [Package Updates](#package-updates)
4. [Package Removal](#package-removal)
5. [Package Information](#package-information)

## Basic Package Management Commands

- `pkg`
  - The primary command for package management in Termux.
  - Example: `pkg update` (updates the package list).

- `apt`
  - The underlying package management tool used by Termux, compatible with `pkg`.
  - Example: `apt update` (updates the package list).

## Package Installation

- `pkg install`
  - Installs a package.
  - Example: `pkg install vim` (installs the Vim text editor).

- `apt install`
  - An alternative to `pkg install` for installing packages.
  - Example: `apt install git` (installs Git version control system).

## Package Updates

- `pkg update`
  - Updates the list of available packages and their versions.
  - Example: `pkg update` (fetches the latest package information).

- `apt update`
  - An alternative to `pkg update` for updating package lists.
  - Example: `apt update` (updates package information).

- `pkg upgrade`
  - Upgrades installed packages to their latest versions.
  - Example: `pkg upgrade` (updates all installed packages).

- `apt upgrade`
  - An alternative to `pkg upgrade` for upgrading packages.
  - Example: `apt upgrade` (upgrades all installed packages).

## Package Removal

- `pkg uninstall`
  - Removes a package.
  - Example: `pkg uninstall vim` (removes the Vim text editor).

- `apt remove`
  - An alternative to `pkg uninstall` for removing packages.
  - Example: `apt remove git` (removes Git).

- `apt purge`
  - Removes a package and its configuration files.
  - Example: `apt purge vim` (removes Vim and its configuration files).

## Package Information

- `pkg search`
  - Searches for a package by name.
  - Example: `pkg search nano` (searches for the Nano text editor).

- `apt search`
  - An alternative to `pkg search` for finding packages.
  - Example: `apt search curl` (searches for the `curl` package).

- `pkg info`
  - Displays information about a package.
  - Example: `pkg info vim` (shows details about the Vim package).

- `apt show`
  - An alternative to `pkg info` for package details.
  - Example: `apt show git` (provides information about the Git package).

- `pkg list-installed`
  - Lists all installed packages.
  - Example: `pkg list-installed` (displays all installed packages).

- `dpkg -l`
  - Lists all installed packages (dpkg command).
  - Example: `dpkg -l` (shows a list of installed packages).

## Conclusion

These commands help manage software packages efficiently in Termux. For more detailed usage and options, refer to the respective command's manual page (e.g., `man pkg` or `man apt`).

Happy package managing!
