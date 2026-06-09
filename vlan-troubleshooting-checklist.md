# VLAN Troubleshooting Checklist

## Verify VLAN Configuration

- Check VLAN exists on the switch
- Verify VLAN ID is correct
- Confirm VLAN is active

## Check Port Assignments

- Verify access ports are assigned to the correct VLAN
- Confirm trunk ports allow the required VLANs
- Check native VLAN configuration

## Validate Connectivity

- Test communication between devices in the same VLAN
- Verify default gateway reachability
- Confirm inter-VLAN routing if required

## Common Issues

- Incorrect VLAN assignment
- VLAN not allowed on trunk
- Native VLAN mismatch
- STP blocking the port
- Missing inter-VLAN routing configuration

## Useful Commands

### Cisco

- show vlan brief
- show interfaces trunk
- show spanning-tree
- show ip interface brief

### Juniper

- show vlans
- show ethernet-switching table
- show interfaces terse

## Best Practices

- Document VLAN assignments
- Use consistent VLAN naming conventions
- Regularly audit trunk configurations
- Remove unused VLANs
