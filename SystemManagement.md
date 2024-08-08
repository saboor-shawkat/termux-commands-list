# System Management Commands in Termux

System management commands help in maintaining, configuring, and monitoring your Termux environment. This document provides an overview of essential system management commands.

## Table of Contents

1. [System Information](#system-information)
2. [User and Group Management](#user-and-group-management)
3. [Service Management](#service-management)
4. [System Logs](#system-logs)
5. [System Configuration](#system-configuration)

## System Information

- `uname`
  - Displays system information.
  - Example: `uname -a` (shows all available system information).

- `arch`
  - Displays the machine architecture.
  - Example: `arch` (shows the system architecture, e.g., `aarch64`).

- `uptime`
  - Shows how long the system has been running.
  - Example: `uptime` (displays the system’s uptime and load averages).

- `top`
  - Provides real-time system resource usage and process information.
  - Example: `top` (shows a dynamic view of system processes and resource usage).

- `df`
  - Displays disk space usage.
  - Example: `df -h` (shows disk space usage in a human-readable format).

- `free`
  - Shows memory usage statistics.
  - Example: `free -h` (displays memory usage in a human-readable format).

## User and Group Management

- `whoami`
  - Displays the current user’s username.
  - Example: `whoami` (shows the username of the current user).

- `id`
  - Displays user and group IDs.
  - Example: `id` (shows user and group information for the current user).

- `groups`
  - Lists groups the current user is part of.
  - Example: `groups` (lists groups for the current user).

- `passwd`
  - Changes user password.
  - Example: `passwd` (prompts to change the password for the current user).

- `su`
  - Switches users (requires root access).
  - Example: `su` (switches to the root user).

## Service Management

- `termux-reload-settings`
  - Reloads Termux settings without restarting.
  - Example: `termux-reload-settings` (reloads settings for Termux).

- `termux-wake-lock`
  - Prevents the device from sleeping.
  - Example: `termux-wake-lock` (prevents the screen from turning off).

- `termux-wake-unlock`
  - Allows the device to sleep.
  - Example: `termux-wake-unlock` (releases the wake lock).

- `service`
  - Manages Android services (requires `termux-service`).
  - Example: `service --status` (lists services status, if available).

## System Logs

- `logcat`
  - Displays system log messages.
  - Example: `logcat` (shows real-time system logs).

- `dmesg`
  - Prints kernel ring buffer messages.
  - Example: `dmesg` (displays kernel messages from the ring buffer).

## System Configuration

- `settings`
  - Accesses and modifies Android system settings (requires root).
  - Example: `settings list system` (lists system settings).

- `pm`
  - Manages application packages (requires root).
  - Example: `pm list packages` (lists all installed packages).

- `top`
  - Provides detailed system resource usage (also used for monitoring).
  - Example: `top` (shows CPU, memory usage, and active processes).

## Conclusion

These commands are fundamental for managing and configuring your Termux environment. For more detailed usage and options, refer to the respective command's manual page (e.g., `man top` or `man df`).

Happy managing!
