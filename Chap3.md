# Scanning
______________________________________________

2nd step in the attack lifecycle.\
Make sure the host is available.
 - Scanning IPs
 - Identifying open ports.
 - Identifying services running on default ports
 - Check against DBs.
 - Try to identify the version and show its CVEs otherwise they show all CVEs for the service.
 - Identify ping by 
   - TTL (Time To Live)
     - 128 for Windows.
     - 64 for Linux.
   - TCP windows : more accurate
<br>
<br>
 - Legion : Collection of tools.
 - Nessus
 - Coalis
 - metasploit

### Types of scanning
 - Port scanning
 - Host / network scanning
 - Network scanning

### Tools
 - nmap
   - -o minimum information
   - chneck open posrt and running services
   - change config
   - request cooldown
   - mimic traffic
   - default port : 40125
 - Zenmap : GUI for nmap
 - Hping2 / Hping3
   - CLI for network crafting
   - regular scans
     - ICMP
     - ACK (TCP)
     - UDP
     - scene scans
     - SIN an entire range
     - intercept traffic
   - DoS : SIN Flooding
 - metasploit

### Host discovery techniques
 - ARP :
   - table for IP - MAC address resolution\
   - ARP spoofing.
   - 192.168.  /  172.  /  10.  Non routable IPs. Decided by the DHCP

- Sweep scanning. (ping different hosts)
- nmap -PA => ACK
- TCP
    - Full open scan : 3-way handshakr \
                           > sync < ack > sync ack > reset
    - Half : > sync < ack > reset

_______________________________________

## Side notes
 - Port forwarding : from router to specific internal IP\
 - DMZ
 - DHCP not used for servers.
 - RFC 1918
   <br>
   <br>
   137 - 138 - 139 : net bios
   445 : SMB
   <br>
   <br>
   3 way handshake
   <br>
   <br>
   UDP : there's aresponse but we dont care.
   <br>
   <br>
   TTL 64   -> TTL exeeded\
   -> time out\
   TTL : number of hops in the network (nombre de relais)\
   Host unreachable :  DHCP problem\
   Routing problem\

Trlnet : 23\
FTP : 20 - 21 (auth - data)\
SSH : 22  /  2222\
SMTP : 25\
Merberos : 88\
SFTP : 22\
RDP : 3389\
NTP : synchronisation du temps 123
Elastic search : 9200
