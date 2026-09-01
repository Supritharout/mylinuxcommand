# Linux and Network Command for every day Use.



### *Connectivity Testing*
1. **ping** google.com - checks if host is reachable
2. **traceroute/tracepath** (traceroute google.com) - Show the path (hops) packets take to reach a destination, useful for finding where connectivity breaks
3. **curl** (curl -I https://example.com) - Test HTTPS/HTTPS endpoints.API
4. **wget** (wget https://example.com/file.zip) - Download files/test if a URL is reachable

### *DNS Troubleshooting*
1. **nslookup** (nslookup google.com) - To query the DNS record
2. **dig**(dig google.com) - More detailed DNS lookup(preferred by most sysadmins over nslookup)
3. **host** (host google.com) - Simple DNS lookup.

### *Port and connection checks*
1. **telent** (telnet example.com 443) - Test if a specific port is open/reachable
2. **ss** - Show active connections and listening ports (modern replacement for netstat)
      1. (ss -tuln # show all listening tcp/udp port) 
      2. (ss -tunap #show with process names with sudo)
3. **netstat** -tulnp

### *Interface and IP Configuration*
1. **ip addr / ip a** - Show network interface and IP address, modern replacement for ifconfig)
2. **ip route** - Show routing table
