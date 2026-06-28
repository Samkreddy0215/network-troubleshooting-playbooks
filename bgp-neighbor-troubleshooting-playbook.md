# BGP Neighbor Troubleshooting Playbook

## Overview

This playbook provides a step-by-step process for diagnosing BGP neighbor establishment and route exchange issues.

## Common Symptoms

- BGP neighbor remains in Idle or Active state
- Neighbor flapping
- Routes not being learned
- Routes not being advertised

## Verification Commands

### Cisco IOS

show ip bgp summary
show ip bgp neighbors
show ip route bgp
show tcp brief

### Palo Alto

show routing protocol bgp summary
show routing protocol bgp peer

## Troubleshooting Workflow

### 1. Verify IP Connectivity

- Ping the neighbor IP
- Verify routing to the peer
- Check interface status

### 2. Verify BGP Parameters

- Neighbor IP
- Remote AS
- Local AS
- Update-source configuration

### 3. Check TCP Connectivity

- Confirm TCP port 179 is reachable
- Verify no firewall or ACL is blocking the session

### 4. Validate Route Exchange

- Confirm expected prefixes are advertised
- Verify inbound and outbound routing policies
- Check prefix lists and route maps

## Common Root Causes

- Incorrect remote AS
- Neighbor IP mismatch
- Missing update-source
- ACL or firewall blocking TCP 179
- Route filtering policies
- Authentication password mismatch

## Best Practices

- Use loopback interfaces with update-source
- Implement prefix filtering
- Enable BFD where appropriate
- Monitor neighbor stability
- Document peering policies and AS numbers
