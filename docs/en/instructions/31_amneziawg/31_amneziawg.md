
# AmneziaWG

A modern version of the popular WireGuard VPN protocol. 
AmneziaWG is a fork of [WireGuard-Go]. It is protected from detection by DPI systems, while retaining the simplified architecture and high performance of the original.

AmneziaWG's progenitor, WireGuard, is known for its performance, but it has detection problems due to its distinctive packet signatures.
AmneziaWG solves this problem by using more advanced obfuscation techniques so that its traffic blends in with normal Internet traffic. \
In this way, AmneziaWG maintains high performance while adding an extra layer of stealth, making it a great choice for those who need a fast and stealthy VPN connection.

- Available with AmneziaVPN on all platforms. 
- Low power consumption. 
- Minimal configuration. 
- Not recognised by DPI analysis systems, resistant to blocking. 
- Works over UDP network protocol.

**Principle of operation.**

AmneziaWG works within the framework of backward compatibility. That is, the AmneziaWG implementation allows you to change some static parameters in WireGuard, by which the protocol is usually recognised by DPI systems. And if these parameters are left as default (equal to 0), the protocol will work as a normal WireGuard.

In AmneziaWG the headers of all packets have been changed: 
- handshake packet (Initiator to Responder), 
- response packet (Responder to Initiator), 
- data packet, as well as 
- special packet "Under Load" - by default they are random values, but you can change them in the settings.

Since every user has different headers, it is impossible to write a universal rule based on headers for tracking systems to calculate the protocol and block it.

Another weak point of WireGuard is the size of the authorisation packets. \
AmneziaWG adds random bytes to each auth packet to change its size. \
So the "init and response packets" of the handshake additionally have a "rubbish" at the beginning of the data, the size of which is determined by the values S1 and S2.\.
By default, the initiating handshake packet has a fixed size (148 bytes), and after adding rubbish, its size will be 148 bytes +S1. \
The AmneziaWG implementation also provides another trick for more robust masking. Before starting a session, Amnezia sends a number of "rubbish" packets to confuse DPI systems to the extreme. The number of such packets and their minimum and maximum size in bytes is also set in the settings, with parameters Jc, Jmin and Jmax.

Links:

[WireGuard-Go] 

Supporting utilities:

[For Android]   
[For Windows]   
[For MacOS и IOS]     
[For Wireguard] 


If you still have questions, please refer to [FAQ], our [telegram chat] or [other sections of the manual].

[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
[FAQ]: ../faq 
[telegram chat]: https://t.me/amnezia_vpn
[other sections of the manual]:  ../instructions
[WireGuard-Go]: https://github.com/amnezia-vpn/amnezia-wg
[For Android]: https://github.com/amnezia-vpn/awg-android
[For Windows]: https://github.com/amnezia-vpn/awg-windows
[For MacOS и IOS]: https://github.com/amnezia-vpn/awg-apple
[For Wireguard]: https://github.com/amnezia-vpn/amnezia-wg-tools





















