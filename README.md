# he-4to6-tunnel

Assists in setting up a Hurricane Electric IP4-to-IP6 tunnel given
configuration parameters yielded upon signup & creation.

## Requirements
- This only works for Debian-based distros
- Your `/etc/network/interfaces` must be configured with:

    ```
    source /etc/network/interfaces.d/*.cfg
    ```

## Role Variables

### Required Variables
- `he4to6_endpoint_ipv4` - Labeled "Server IPv4 Address"
- `he4to6_endpoint_ipv6` - Labeled "Server IPv6 Address" *(without CIDR)*
- `he4to6_local_addr` - Labeled "Client IPv4 Address" The IPv4 WAN address
you'll be connecting from.
- `he4to6_addr` - Labeled "Client IPv6 Address" *(without CIDR)*

### Default Variables
- `he4to6__iface_name` - Interface name (Defaults to `hurricane0`)
- `he4to6__timeout_ifdown` - Number of seconds to wait while calling `ifdown`
when cycling the interface
- `he4to6__timeout_ifup` - Number of seconds to wait while calling `ifup` when
cycling the interface
- `he4to6__ttl` - TTL (Defaults to 255)

## Dependencies
*N/A*

## License
BSD
