# AmneziaWG

[AmneziaWG] is a contemporary version of the popular VPN protocol, WireGuard. It's a fork of [WireGuard-Go] and offers protection against detection by Deep Packet Inspection (DPI) systems. At the same time, it retains the simplified architecture and high performance of the original.

The precursor, WireGuard, is known for its efficiency but had issues with detection due to its distinctive packet signatures. \
AmneziaWG addresses this problem by employing advanced obfuscation methods, allowing its traffic to blend seamlessly with regular internet traffic. \
As a result, AmneziaWG maintains high performance while adding an extra layer of stealth, making it a superb choice for those seeking a fast and discreet VPN connection.

Features of AmneziaWG include:

- Availability with AmneziaVPN on all platforms.
- Low energy consumption.
- Minimal configuration needed.
- Undetectable by DPI analysis systems, resistant to blocking.
- Operates over the UDP network protocol.


### Working Principle: ###

AmneziaWG operates with backward compatibility. This means that the AmneziaWG implementation allows for modifications to certain static parameters in WireGuard, which are typically recognized by DPI systems. If these parameters are left at their default values (equal to 0), the protocol functions like standard WireGuard.

In AmneziaWG, headers of all packets have been modified:

- Initiator to Responder.
- Responder to Initiator.
- Data packet.
- Special "Under Load" packet – by default, random values are set, but these can be manually adjusted in the settings.


Since every user has different headers, it's nearly impossible to draft a universal tracking rule based on these headers to detect and block the protocol.

Another vulnerability of WireGuard lies in the sizes of its authentication
packets. \
In AmneziaWG, random bytes are appended to every auth packet to alter their size. \
Thus, "init and response handshake packets" have added "junk" at the beginning of their data, the size of which is determined by the values S1 and S2. \
By default, the initiating handshake packet has a fixed size (148 bytes). After adding the junk, its size becomes 148 bytes + S1. \
AmneziaWG also incorporates another trick for more reliable masking. Before initiating a session, Amnezia sends a certain number of "junk" packets to thoroughly confuse DPI systems. The number of these packets and their minimum and maximum byte sizes can also be adjusted in the settings, using parameters Jc, Jmin, and Jmax.

If you have further questions, please refer to the FAQ, our Telegram chat, or other sections of the instruction manual.


Links:

[AmneziaWG] - main repository

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
[AmneziaWG]: https://github.com/amnezia-vpn/amnezia-wg
[For Android]: https://github.com/amnezia-vpn/awg-android
[For Windows]: https://github.com/amnezia-vpn/awg-windows
[For MacOS и IOS]: https://github.com/amnezia-vpn/awg-apple
[For Wireguard]: https://github.com/amnezia-vpn/amnezia-wg-tools
[WireGuard-Go]: https://github.com/WireGuard/wireguard-go






