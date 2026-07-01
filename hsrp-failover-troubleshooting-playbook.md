# HSRP Failover Troubleshooting Playbook

## Overview

This playbook provides a structured approach to troubleshooting HSRP failover and gateway redundancy issues in Cisco enterprise networks.

## Common Symptoms

- Virtual gateway unreachable
- Failover not occurring
- Frequent Active/Standby role changes
- Duplicate virtual IP detected

## Verification Commands

### Cisco

show standby brief
show standby
show ip interface brief
show logging

## Troubleshooting Workflow

### Verify Interface Status

- Confirm physical interfaces are up
- Verify VLAN interface status
- Check Layer 2 connectivity

### Verify HSRP Configuration

- Virtual IP address
- Group number
- Priority
- Preemption
- Authentication

### Validate Network Connectivity

- Ping virtual IP
- Verify default gateway
- Confirm ARP table entries

### Check Failover

- Shutdown active interface
- Verify standby becomes active
- Confirm traffic continues without interruption

## Common Root Causes

- Priority mismatch
- Preemption disabled
- Authentication mismatch
- Interface tracking failure
- VLAN or trunk issues

## Best Practices

- Enable preemption
- Track WAN interfaces
- Use authentication
- Monitor HSRP state changes
- Test failover periodically
