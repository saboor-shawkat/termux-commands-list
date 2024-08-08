# System Monitoring Commands in Termux

System monitoring is essential for understanding how your Termux environment is performing. This document provides an overview of common commands used to monitor system resources and performance.

## Table of Contents

1. [Basic System Monitoring Commands](#basic-system-monitoring-commands)
2. [CPU and Memory Usage](#cpu-and-memory-usage)
3. [Disk Usage and Space](#disk-usage-and-space)
4. [Process Management](#process-management)
5. [Network Statistics](#network-statistics)

## Basic System Monitoring Commands

- `top`
  - Displays real-time system information and processes.
  - Example: `top` (shows a dynamic, real-time view of system processes and resource usage).

- `htop`
  - An enhanced version of `top` with a more user-friendly interface (may need installation).
  - Example: `htop` (provides an interactive view of system processes).

- `uptime`
  - Shows how long the system has been running, along with average load.
  - Example: `uptime` (displays the system's uptime and load averages).

## CPU and Memory Usage

- `free`
  - Displays memory usage statistics.
  - Example: `free -h` (shows memory usage in human-readable format).

- `vmstat`
  - Reports virtual memory statistics.
  - Example: `vmstat 1` (provides a continuous display of system performance metrics every second).

- `mpstat`
  - Shows CPU usage statistics (part of `sysstat` package).
  - Example: `mpstat` (displays CPU utilization for each processor).

- `sar`
  - Collects and reports system activity information (part of `sysstat` package).
  - Example: `sar -u 1` (shows CPU utilization every second).

## Disk Usage and Space

- `df`
  - Reports disk space usage for all mounted filesystems.
  - Example: `df -h` (shows disk usage in human-readable format).

- `du`
  - Estimates file and directory space usage.
  - Example: `du -sh /path/to/directory` (displays the total size of the specified directory).

- `lsblk`
  - Lists information about block devices.
  - Example: `lsblk` (displays information about disk drives and partitions).

## Process Management

- `ps`
  - Displays information about active processes.
  - Example: `ps aux` (shows detailed information about all running processes).

- `kill`
  - Sends a signal to terminate a process.
  - Example: `kill -9 PID` (forcefully terminates the process with process ID `PID`).

- `pkill`
  - Sends a signal to processes by name.
  - Example: `pkill firefox` (terminates all processes with the name `firefox`).

- `pgrep`
  - Searches for processes based on criteria.
  - Example: `pgrep -fl firefox` (lists process IDs and names for processes matching `firefox`).

## Network Statistics

- `netstat`
  - Displays network connections, routing tables, and interface statistics.
  - Example: `netstat -tuln` (shows listening ports and associated processes).

- `ss`
  - Utility to investigate sockets (more modern than `netstat`).
  - Example: `ss -tuln` (displays listening sockets with TCP and UDP).

- `iftop`
  - Displays bandwidth usage on network interfaces (requires installation).
  - Example: `iftop` (provides a real-time view of network traffic).

- `nload`
  - Monitors network traffic and bandwidth usage (requires installation).
  - Example: `nload` (shows incoming and outgoing traffic in real-time).

## Conclusion

Monitoring system performance and resources is crucial for maintaining a healthy Termux environment. For more detailed information and options, refer to the respective command's manual page (e.g., `man top` or `man df`).

Happy monitoring!
