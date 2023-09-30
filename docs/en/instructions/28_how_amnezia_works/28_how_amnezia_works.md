# Принцип работы Amnezia


&nbsp;

###  What is AmneziaVPN?

 AmneziaVPN is a free open-source multi-protocol VPN client with the function of setting up your own VPN server, or in other words self-hosted VPN.


### How does Amnezia create a VPS-based VPN?

When you connect for the first time, the application automatically generates a new key pair for OpenVPN and
generates a Certificate Signing Request (CSR). The Certificate Signing Request, 
including the public key, is then passed to the server for signing and issuing the corresponding 
X.509 certificate that provides authentication and security for the connection.



###  How does Amnezia connect to the created VPN?

After the user enters the IP login and password from the VPS, the application 
connects to the server via SSH and installs Docker and runs the Amnezia server containers.
SSH, installs Docker, and runs the Amnezia server containers. For each protocol
connection, a separate container is started, keys and root certificate are generated.
Once the server is configured, you can connect using VPN to that server.

###  How does traffic masking work ?

ShadowSocks and OpenVPN over cloak protocols have traffic cloaking 

ShadowSock is based on the SOCKS5 proxy protocol, which protects the connection using the AEAD cipher - roughly along the same lines as SSH tunneling. A Shadowsocks connection is difficult to identify because it is virtually identical to a normal HTTPS connection.
However, some traffic analysis systems can still recognize a ShadowSocks connection, so in countries with high levels of censorship we recommend using OpenVPN in conjunction with Cloak.

In OpenVPN over Cloak, the Cloak plugin is responsible for traffic masking. It can modify packet metadata in such a way that it completely masks VPN traffic as regular web traffic and also protects the VPN from detection by Active Probing. This makes it very resistant to detection and blocking. Immediately after receiving the first data packet, Cloak authenticates the incoming connection. In case the authentication fails, the plugin masks the server as a fake website and your VPN becomes invisible to analysis systems. 

If there is a high level of Internet censorship in your region, we advise you to use only OpenVPN over Cloak from the first connection


###  The principle of operation of most commercial VPNs
###  Amnezia VPN working principle
()

If you still have questions, please refer to [FAQ], our [telegram chat] or [other sections of the manual]

[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
[FAQ]: /about 
[telegram chat]: /about 
[other sections of the manual]: /about



















