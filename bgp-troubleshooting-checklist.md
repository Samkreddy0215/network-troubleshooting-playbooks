# BGP Troubleshooting Checklist

## Verify Neighbor Status

- show ip bgp summary
- show bgp ipv4 unicast summary
- Verify Established state

## Check Reachability

- Ping neighbor IP
- Verify routing to neighbor
- Confirm source interface configuration

## Validate BGP Configuration

- Neighbor IP
- Remote AS
- Update-source settings
- Authentication settings

## Route Advertisement Checks

- show ip bgp
- show ip bgp neighbors advertised-routes
- show ip bgp neighbors received-routes

## Common Issues

- ASN mismatch
- Authentication mismatch
- ACL or firewall blocking TCP 179
- Missing network statements
- Incorrect route filtering

## Useful Commands

- show ip route
- show ip bgp summary
- show ip bgp neighbors
- debug ip bgp
