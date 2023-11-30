# Firewalls_IPSec

Following the lab on the Juniper website below. Route-based VPN.

https://www.juniper.net/documentation/us/en/software/junos/vpn-ipsec/topics/topic-map/security-route-based-ipsec-vpns.html

Sandbox: https://jlabs.juniper.net/vlabs/portal/ipsec-vpn-route-based/

<p>
v1: Set up a basic VPN Tunnel that allowed VPN communication through static routes.<br>
v2: Added BGP to allow oobsr and oobhr to exchange VPN routes via BGP instead of static routes.<br>
v3: Added SNAT to allow hosts to communicate to the internet.<br>
v4: Changed set of IKE and IPsec proposals from standard to custom proposal set of encryption and authentication algorithms.<br>
v5: Changed internet-to-SRX policies from protocol-based to application-based polices for deep-packet inspection. Only ICMP, SSH from COPR-Address, IKE and IPSEC permitted.
v6: Added IDS to protect against IP, TCP and ICMP attacks from internet; updated oobhr to only advertise 10.0.0.0/8 aggregate prefix; removed static VPN prefixes.
<p>