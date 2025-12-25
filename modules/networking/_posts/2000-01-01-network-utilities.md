---
title: Windows Networking Utilities
---
## Windows Networking Utilities

### Identifying Network Connections

The external `nmap` scan is a brief check for the most common running services on your Windows server, but how do you get info from within the OS? Additionally, if Red Team opens up more backdoors on your system, how do you find them?

The `netstat` command lists all active network connections and ports your computer is listening on. If there's an active outbound connection, or if there's a service listening on a port for an inbound connection, `netstat` will show you it. 

The most common options I use are:
`netstat -abo` (List all connections/listening ports, show which executable created the connection, include the process ID)

Alternatively, [TCPView](https://learn.microsoft.com/en-us/sysinternals/downloads/tcpview) is a GUI tool that you can download to show the exact same things.

### Troubleshooting Utilities
You may find these tools useful when your Internet connection drops or if a service goes down for whatever reason.

* `ping` / `tracert` - Check if a connection is up and the path to it
* `nslookup` - DNS Resolver
* `arp` - ARP Cache + Resolver