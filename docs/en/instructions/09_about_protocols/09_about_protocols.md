# Description of protocols

### About protocols

> We do not recommend using OpenVPN, Wireguard, IKEv2 protocols without traffic masking in countries
with high level of censorship, as the ip address of your VPS may be blocked. To avoid blocking use only
OpenVPN over Cloak.


### OpenVPN  

The time-tested most popular VPN protocol.  Uses proprietary security protocol with SSL/TLS for encryption
and key exchange and supports various authentication methods, making it suitable for different devices and
operating systems.

Normal power consumption on mobile devices. \
Flexible customization to meet user needs to work with different operating systems and devices. \
Recognized by DPI analysis systems, and therefore susceptible to blocking. \
Can operate over both TCP and UDP network protocols. 

### ShadowSocks


It is based on the SOCKS5 proxy protocol, which protects the connection using the AEAD cipher - roughly
along the same lines as SSH tunneling. A Shadowsocks connection is difficult to identify because it is
virtually identical to a normal HTTPS connection.
However, some traffic analysis systems can still recognize a ShadowSocks connection, so in countries with
high levels of censorship we recommend using OpenVPN in conjunction with Cloak.

Average power consumption on mobile devices (higher than OpenVPN). \
It is possible to customize the encryption protocol. \
Recognized by some DPI analysis systems  \
Works only via TCP network protocol



###  OpenVPN over Cloak

It is based on the SOCKS5 proxy protocol, which protects the connection using the AEAD cipher - roughly
along the same lines as SSH tunneling. A Shadowsocks connection is difficult to identify because it is
virtually identical to a normal HTTPS connection.
However, some traffic analysis systems can still recognize a ShadowSocks connection, so in countries with
 high levels of censorship we recommend using OpenVPN in conjunction with Cloak.

Average power consumption on mobile devices (higher than OpenVPN). \
It is possible to customize the encryption protocol. \
Recognized by some DPI analysis systems \
Works only via TCP network protocol

 penVPN over Cloak versions installed on client versions younger than 3 are not compatible with > subsequent versions of the client. 
subsequent versions of the client. If you installed OpenVPN over Cloak on version 1 or 2 of the client, you must reinstall the protocol to make it work on versions 3 and 4.

 ###  WireGuard

Relatively new popular VPN protocol with simplified architecture. 
Provides stable VPN connection, high performance on all devices. Uses hard-coded encryption settings. 
WireGuard compared to OpenVPN has lower latency and better data throughput.

Low power consumption on mobile devices. \
Minimum number of settings. \
Easily recognized by DPI analysis systems, susceptible to blocking. \
Works via UDP network protocol.

###  IKEv2

Modern stable protocol. IKEv2 with IPSec encryption layer. Transmits data over fixed UDP ports 500 and
4500 protecting them with strong 3DES and AES crypto algorithms. Allows very fast switching between networks and devices. Due to its security, stability and speed, IKEv2 is currently one of the best VPN solutions for mobile devices. Vulnerable to detection and blocking.


Low power consumption, on mobile devices \
Minimal amount of customization. \
Recognized by DPI analysis systems. \
Works only over UDP network protocol 




###  AmneziaWG
A modern iteration of the popular VPN protocol, AmneziaWG builds upon the foundation set by WireGuard, retaining its simplified architecture and               high-performance capabilities across devices.
While WireGuard is known for its efficiency, it had issues with being easily detected due to its distinct packet signatures. AmneziaWG solves this problem by using better obfuscation methods, making its traffic blend in with regular internet traffic.
This means that AmneziaWG keeps the fast performance of the original while adding an extra layer of stealth, making it a great choice for those wanting a fast and discreet VPN connection.

Available in the AmneziaVPN across all platforms Low power consumption \
Minimum number of settings. \
Not recognised by DPI analysis systems, resistant to blockingю. \
Works over UDP network protocol.

If you still have questions, please refer to [FAQ], our [Telegram chat] or [other sections of the manual]


[about-int-link]: /about
[FAQ]: ../faq 
[Telegram chat]: https://t.me/amnezia_vpn_en
[other sections of the manual]: ../instructions









