# Palo Alto Firewall Troubleshooting Playbook

## Common Connectivity Issues

### Traffic Blocked Unexpectedly

Check:

- Security policy rules
- Source and destination zones
- Application identification
- Service and port configuration

Commands:

```bash
show running security-policy
show session all filter source <ip>
