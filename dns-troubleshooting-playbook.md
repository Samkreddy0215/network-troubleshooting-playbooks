# DNS Troubleshooting Playbook

## Objective

Identify and resolve DNS resolution issues affecting applications, servers, and end users.

## Initial Checks

1. Verify IP connectivity
2. Confirm DNS server reachability
3. Check DNS client configuration
4. Validate default gateway

## Common Commands

### Windows

nslookup google.com
ipconfig /all
ipconfig /flushdns

### Linux

dig google.com
nslookup google.com
cat /etc/resolv.conf

### Cisco

show hosts
ping dns-server-ip

## Troubleshooting Workflow

1. Test name resolution
2. Compare internal and external lookups
3. Verify DNS records
4. Check firewall policies
5. Review DNS server logs
6. Validate forwarders and zones

## Common Causes

- Incorrect DNS server settings
- Expired DNS records
- Firewall blocking DNS traffic
- DNS service outage
- Split-brain DNS configuration issues

## Resolution Validation

- Successful hostname resolution
- Application connectivity restored
- DNS response times within normal range
- No recurring lookup failures
