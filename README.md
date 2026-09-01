# Linux and Network Command for every day Use.



### *Connectivity Testing*
1. ping google.com - checks if host is reachable
2. traceroute/tracepath (traceroute google.com) - Show the path (hops) packets take to reach a destination, useful for finding where connectivity breaks
3. curl (curl -I https://example.com) - Test HTTPS/HTTPS endpoints.API
4. wget (wget https://example.com/file.zip) - Download files/test if a URL is reachable

### *DNS Troubleshooting*
1. nslookup (nslookup google.com) - To query the DNS record
2. dig(dig google.com) - More detailed DNS lookup(preferred by most sysadmins over nslookup)
3. host (host google.com) - Simple DNS lookup.

### *Port and connection checks*
1. telent (telnet example.com 443) - Test if a specific port is open/reachable
2. ss (ss -tuln # show all listening tcp/udp port) - Show active connections and listening ports (modern replacement for netstat)
      (ss -tunap #show with process names with sudo)
