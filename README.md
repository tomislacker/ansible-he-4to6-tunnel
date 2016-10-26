# he-4to6-tunnel

Assists in setting up a Hurricane Electric IP4-to-IP6 tunnel given
configuration parameters yielded upon signup & creation.

## Requirements
*N/A*

## Role Variables

### Required Variables
- `he4to6_endpoint_ipv4` - Labeled "Server IPv4 Address"
- `he4to6_endpoint_ipv6` - Labeled "Server IPv6 Address" *(without CIDR)*
- `he4to6_local_addr` - Labeled "Client IPv4 Address" The IPv4 WAN address
you'll be connecting from.
- `he4to6_addr` - Labeled "Client IPv6 Address" *(without CIDR)*

### Default Variables
- `he4to6__iface_name` - Interface name (Defaults to `hurricane0`)
- `he4to6__ttl` - TTL (Defaults to 255)

## Dependencies
*N/A*

## License
BSD
