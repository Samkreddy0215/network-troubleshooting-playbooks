# OSPF Troubleshooting Playbook

## Common OSPF Issues

### Neighbor Adjacency Not Forming

Check:

- IP connectivity between neighbors
- OSPF enabled on interfaces
- Area IDs match
- Hello/Dead timers match
- Authentication settings match
- MTU values match

Commands:

```bash
show ip ospf neighbor
show ip ospf interface
show ip protocols
