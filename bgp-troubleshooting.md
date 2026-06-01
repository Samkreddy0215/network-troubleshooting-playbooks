# BGP Troubleshooting Playbook

## Common BGP Issues

### BGP Neighbor Down

Check:

- IP reachability to peer
- Correct remote AS number
- Neighbor IP configuration
- Firewall rules allowing TCP port 179

Commands:

```bash
show ip bgp summary
show ip bgp neighbors
ping <neighbor-ip>
