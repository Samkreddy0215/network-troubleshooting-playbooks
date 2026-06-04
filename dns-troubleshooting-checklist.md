# DNS Troubleshooting Checklist

## Verify DNS Resolution

- nslookup example.com
- dig example.com
- Verify correct IP address is returned

## Check DNS Server Reachability

- Ping DNS server
- Verify routing to DNS server
- Confirm firewall rules allow DNS traffic

## Validate Client Configuration

- Check configured DNS servers
- Verify DHCP-assigned DNS settings
- Confirm DNS suffix/search domain settings

## Test Record Types

- A Records
- AAAA Records
- CNAME Records
- MX Records
- PTR Records

## Common Issues

- Incorrect DNS server configuration
- Stale DNS cache
- Missing or incorrect DNS records
- Firewall blocking UDP/TCP 53
- Replication issues between DNS servers

## Useful Commands

- nslookup
- dig
- ipconfig /flushdns
- ipconfig /displaydns
- systemd-resolve --status
