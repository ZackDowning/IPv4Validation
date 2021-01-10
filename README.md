# MAC-IP-Address-Validator
Validate MAC address, IPv4 address, and IPv6 formatting using concise Regular Expressions.

The validator module is broken into 3 functions: ipv4, ipv6, and macaddress
The functions return bool if given address formatting is valid.

The modules support the following formats:
IPv4 Address - Dotted Decimal
IPv6 Address - Colon-Seperated Hexadecimal (Hextet)
MAC Address - 'Colon', 'Dash', and 'Period'(Cisco) Seperators with Hexadecimal

All hexadecimal case combinations are supported.

Example usage:
from mac-ip-address-validator import ipv4

ipv4address = '10.0.100.0'
ipv4(ipv4address)
True

ipv6address = 'fe80:::1'
ipv6(ipv6address)
False
