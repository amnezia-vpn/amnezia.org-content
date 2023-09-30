# Alternative applications

You do not have to use a VPN created by Amnezia using the Amnezia client. 
Below are alternative clients for some protocols

&nbsp;

### Clients for "OpenVPN"

OpenVPN Connect is the official client for the OpenVPN protocol.
There are versions for Windows, Linux, MacOS, Android, IOS

OpenVPN for Android - unofficial application with a lot of settings,


### Clients for "Shadowsocks"


Shadowsocks - official clients for Windows, macOS and Android + ChromeOS.
More detailed instructions on how to install ShadowSocks with the Cloak plugin and use it in the ShadowSocks app [here].   

ShadowRocket - third-party Shadowsocks client for iPhone and iPad, paid for about 40$



###  Clients for "OpenVPN over Cloak"

> Create a configuration file to unshare connections for the Shadowsocks and Shadowrocket client only on version 2 and 3 of the client, we plan to add this feature to version 4 of Amnezia in the near future. 


Cloak is a plugin for obfuscating traffic and using it with other protocols. AmneziaVPN contains a Shadowsocks container for use through the Shadowsocks client.
For PC platforms
For Windows: "ck-client-windows", there are usually two files labeled "386" (for 32-bit version) and "amd64" (for 64-bit version).
For Linux: "ck-client-linux", there are 10 files (for 32-bit and 64-bit versions) for x86, arm, mips, mipsle, mips_softfloat architectures.
For macOS: can be found on request - "ck-client-darwin", there is a build only for "amd64" (64-bit processors with x86 architecture, not for new Apple M1 processors).
For Android - can be used in the official Shadowsocks client

###  Clients for "Wireguard"

Wireguard is an official client.  There is a version for Windows, Linux, MacOS, IOS, Android, 
also on the official page there is a mention of OpenWRT firmware to install on the router.

###  Clients for "IPSec" (IKEv2)

StrongSwan is a cross-platform IPSec IKEv2 client for Linux, FreeBSD, macOS and Android. Note (export bugfixes required).
There are versions for Windows, Linux, MacOS, Android.

Most modern devices (except Android) have built-in support for IKEv2, and have the ability to configure the connection "out of the box". To connect to them, you need to know the IP address of the server and have a p12 certificate.

If you still have questions, please refer to [FAQ], our [telegram chat] or [other sections of the manual]

[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
[FAQ]: /about 
[telegram chat]: /about 
[other sections of the manual]: /about
[here]


















