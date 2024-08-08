# Networking Commands in Termux

Termux provides a robust terminal environment on Android, and includes a variety of networking commands for managing and troubleshooting network connections. This document covers some of the most commonly used networking commands in Termux.

## Table of Contents

1. [Basic Networking Commands](#basic-networking-commands)
2. [Network Configuration](#network-configuration)
3. [Network Diagnostics](#network-diagnostics)
4. [Networking Tools](#networking-tools)

## Basic Networking Commands

- `ping`
  - Tests connectivity to a remote host.
  - Example: `ping google.com` (sends ping requests to `google.com`).

- `ifconfig` (or `ip addr`)
  - Displays or configures network interfaces.
  - Example: `ifconfig` (lists all network interfaces and their configurations).
  - Example: `ip addr show` (shows network interfaces and IP addresses).

- `netstat`
  - Displays network connections, routing tables, and interface statistics.
  - Example: `netstat -tuln` (shows listening ports and associated processes).

- `hostname`
  - Shows or sets the system's hostname.
  - Example: `hostname` (displays the current hostname).

## Network Configuration

- `ip`
  - A powerful tool for network configuration.
  - Example: `ip link set eth0 up` (brings the `eth0` interface up).
  - Example: `ip addr add 192.168.1.100/24 dev wlan0` (assigns an IP address to `wlan0`).

- `route`
  - Manages the IP routing table.
  - Example: `route -n` (displays the routing table).

- `nmcli`
  - Command-line tool for NetworkManager (if installed).
  - Example: `nmcli dev status` (shows the status of network devices).
  - Example: `nmcli con show` (lists available network connections).

## Network Diagnostics

- `traceroute`
  - Shows the path packets take to reach a destination.
  - Example: `traceroute google.com` (traces the route to `google.com`).

- `nslookup`
  - Queries DNS to obtain domain name or IP address mapping.
  - Example: `nslookup example.com` (fetches IP address for `example.com`).

- `dig`
  - Provides detailed DNS query results.
  - Example: `dig example.com` (queries DNS information for `example.com`).

- `curl`
  - Transfers data from or to a server using various protocols.
  - Example: `curl http://example.com` (fetches the content of `example.com`).

- `wget`
  - Retrieves files from the web.
  - Example: `wget http://example.com/file.zip` (downloads `file.zip` from `example.com`).

## Networking Tools

- `iperf`
  - Measures network bandwidth between hosts (requires installation).
  - Example: `iperf -s` (starts `iperf` in server mode).
  - Example: `iperf -c server_ip` (starts `iperf` in client mode connecting to `server_ip`).

- `nmap`
  - Network scanner used to discover hosts and services on a network.
  - Example: `nmap 192.168.1.0/24` (scans all hosts in the `192.168.1.0/24` network).

- `tcpdump`
  - Captures network packets for analysis.
  - Example: `tcpdump -i wlan0` (captures packets on the `wlan0` interface).

- `mtr`
  - Combines `traceroute` and `ping` to provide network diagnostics.
  - Example: `mtr google.com` (provides a live network trace to `google.com`).

## Conclusion

These commands are essential for managing and diagnosing network issues in Termux. For more detailed usage and additional options, refer to the command's manual page (e.g., `man ping`).

Happy networking!
