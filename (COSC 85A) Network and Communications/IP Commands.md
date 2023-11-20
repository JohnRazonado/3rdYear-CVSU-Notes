Really named as: IP/Networking Commands
>This note isn't polished and summarize yet #inProgress 


```
C:>ping
C:>ipconfig
C:>ipconfig /all
C:>ipconfig /release
C:>ipconfig /renew
C:\>nbtstat –a
```

> This command only works for Windows OS.

><mark style="background: #FFB8EBA6;"><strong>Caution:</strong> when typing from the command prompt you can only type one command per
line, and press Enter after each one to execute it.</mark>

**C:\>arp –a**
- is short for address resolution protocol, It will show the IP address of your
computer along with the IP address and MAC address of your router.

**C:\>hostname**
- This is the simplest of all TCP/IP commands. It simply displays the
name of your computer.

**C:\>ipconfig**
- The ipconfig command displays information about the host (the computer
your sitting at)computer TCP/IP configuration.

**C:\>ipconfig /all**
- This command displays detailed configuration information about your
TCP/IP connection including Router, Gateway, DNS, DHCP, and type of Ethernet
adapter in your system.

**C:\>Ipconfig /renew**
- Using this command will renew all your IP addresses that you are
currently (leasing) borrowing from the DHCP server. This command is a quick problem
solver if you are having connection issues, but does not work if you have been configured
with a static IP address.

**C:\>Ipconfig /release**
- This command allows you to drop the IP lease from the DHCP
server.
> This will temporarily remove all the connection of your network.

**C:\>ipconfig /flushdns**: This command is only needed if you’re having trouble with your
networks DNS configuration. The best time to use this command is after network
configuration frustration sets in, and you really need the computer to reply with flushed.

**C:\>nbtstat –a**: This command helps solve problems with NetBIOS name resolution.
(Nbt stands for NetBIOS over TCP/IP)
Definitions

**C:\netdiag**: [Netdiag](https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/cc731434(v=ws.11)) is a network testing utility that performs a variety of network
diagnostic tests, allowing you to pinpoint problems in your network. Netdiag isn’t
installed by default, but can be installed from the Windows XP CD after saying no to the
install. Navigate to the CD ROM drive letter and open the support\tools folder on the XP
CD and click the setup.exe icon in the support\tools folder.
>It won't work on Windows 10
>![[Pasted image 20231025113833.png]]
>This is an old utility function.

**C:\>netstat**
- Netstat displays a variety of statistics about a computers active TCP/IP
connections. This tool is most useful when you’re having trouble with TCP/IP
applications such as HTTP, and FTP.

**C:\>nslookup**
- Nslookup is used for diagnosing DNS problems. If you can access a
resource by specifying an IP address but not it’s DNS you have a DNS problem.

**C:\>pathping**
- Pathping is unique to Window’s, and is basically a combination of the
Ping and Tracert commands. Pathping traces the route to the destination address then
launches a 25 second test of each router along the way, gathering statistics on the rate of
data loss along each hop.

**C:\>ping**
- Ping is the most basic TCP/IP command, and it’s the same as placing a phone
call to your best friend. You pick up your telephone and dial a number, expecting your
best friend to reply with “Hello” on the other end. Computers make phone calls to each
other over a network by using a Ping command.
The Ping commands main purpose is to place a phone call to another computer on the
network, and request an answer. Ping has 2 options it can use to place a phone call to
another computer on the network. It can use the computers name or IP address.

**C:\>route**
- The route command displays the computers routing table. A typical
computer, with a single network interface, connected to a LAN, with a router is fairly
simple and generally doesn’t pose any network problems. But if you’re having trouble
accessing other computers on your network, you can use the route command to make sure
the entries in the routing table are correct.

**C:\>tracert**
- The tracert command displays a list of all the routers that a packet has to go
through to get from the computer where tracert is run to any other computer on the
internet.