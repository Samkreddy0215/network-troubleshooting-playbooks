# VPN Troubleshooting Playbook

## Site-to-Site VPN Issues

### Tunnel Down

Check:

- Peer IP reachability
- IKE Phase 1 status
- IPsec Phase 2 status
- Pre-shared key configuration
- Encryption and hashing settings

Commands:

```bash
show crypto isakmp sa
show crypto ipsec sa
show vpn-sessiondb
```

---

### Tunnel Up But No Traffic

Check:

- Interesting traffic ACLs
- NAT exemption rules
- Routing configuration
- Security policies

Commands:

```bash
show access-list
show route
show crypto ipsec sa
```

---

### Intermittent VPN Connectivity

Check:

- ISP packet loss
- Tunnel rekey timers
- MTU and fragmentation issues
- Firewall session timeouts

Commands:

```bash
ping
traceroute
show interface
```

---

## Best Practices

- Use strong encryption algorithms
- Monitor tunnel uptime
- Document VPN peers and subnets
- Regularly review VPN logs
