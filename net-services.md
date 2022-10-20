# Network Services 

Understanding, Enumerating, and exploiting vulnerable services.

## SMB - Server Message Block Protocol

Server Message Block Protocol - is a client-server communication protocol used for sharing access to files, printers, serial ports and other resources on a network. [SMB](https://searchnetworking.techtarget.com/definition/Server-Message-Block-Protocol)

The SMB protocol is known as a response-request protocol, meaning that it transmits multiple messages between the client and server to establish a connection. Clients connect to servers using TCP/IP (actually NetBIOS over TCP/IP as specified in RFC1001 and RFC1002), NetBEUI or IPX/SPX. 

### Enumeration

**Port Scanning** Scan for open ports 139 and 445
**Enum4Linux** Enum4linux is a tool used to enumerate SMB shares on both Windows and Linux systems. It is basically a wrapper around the tools in the Samba package and makes it easy to quickly extract information from the target pertaining to SMB. 

`enum4linux [options] ip`

### Exploitation

SMB exploits can be viable through vulnerabilities but in many cases through misconfiguration

`smbclient //IP/SHARE -U USER -p PORT`

`more` - read files
`get` - download files to lcd
`?/help` - to understand a command or list out commands

## Telnet

Telnet is an application protocol which allows you, with the use of a telnet client, to connect to and execute commands on a remote machine that's hosting a telnet server. 

`telnet IP PORT`
